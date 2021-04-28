# Accessing Boku’s Test Environment via Postman

[Postman](https://www.postman.com/product/api-client/) is a developer tool that allows for convenient API testing.

With our Postman collection, developers can quickly test Boku API's without having to worry about the intricacies of [Boku API Authentication](https://github.com/boku-inc/boku-api-docs/blob/main/boku-api-auth/README.md).

1. Download [Postman](https://www.postman.com/downloads/)
2. Download the Boku [Merchant Test Environment](https://raw.githubusercontent.com/boku-inc/boku-api-docs/main/common/postman/Merchant%20Test%20Environment.postman_environment.json) Postman environment
3. Download the [Payment Gateway (LPM)](https://raw.githubusercontent.com/boku-inc/boku-api-docs/main/boku-direct-lpm/postman/Payment%20Gateway%20(LPM).postman_collection.json) Postman collection
4. Within the Postman application, import `Merchant Test Environment.postman_environment.json` and `Payment Gateway (LPM).postman_collection.json`
   ![Import](src/img/Screenshot%20from%202021-04-28%2016-37-31.png)
5. Add your `merchantId`, `keyId` and `apiKey` in the `Merchant Test Environment` environment variables. You can get these values from your account manager.
   ![Import](src/img/Screenshot%20from%202021-04-28%2016-52-05.png)
6. Update the `country`, `currency`, `network` and `paymentMethod` in the `Payment Gateway (LPM)` collection to reflect the wallet you wish to test. You can get a list of wallets from your account manager.
   ![Import](src/img/Screenshot%20from%202021-04-28%2016-38-40.png)

You are now ready to begin testing Boku API's.
