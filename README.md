# Test Automation Framework to support Web and Mobile using WDIO, API using Supertest.
-------------------------------------------------------------------------------------------

## Tech Stack
- [WebdriverIO 7.##.#](https://webdriver.io/)
- [Supertest 6.#.#](https://www.npmjs.com/package/supertest)

## Language
- JavaScript

## Reporting
- Allure
- Junit
- Spec

## Test JS Framework
- Mocha


## Local Environment Setup (Mac OS)
- Install Node

  Run =>  `brew install node`

- Install Appium

  Run =>  `brew install appium`

- Install Appium Dependecies

  Run =>  `npm i -g appium`

- Create Android Emulator

  Run =>   `$ANDROID_HOME/tools/bin/avdmanager create avd -n TestEmulator -d pixel --package "system-images;android-30;google_apis;x86"`

- Create iOS Simulator

  Run => `xcrun simctl list`
  ( Note down the **UDID** of  **iOS v15.2  iPhone 12 mini**. This UDID will be later used in Package Json scripts to invoke Simulator )


## Project Framework Setup in Local

- Clone the Repo from [GitHub](https://github.com/girlCoder8/web-api-mobile-wdio)

  Run => `git clone https://github.com/girlCoder8/web-api-mobile-wdio.git`

  Run => `npm install`


## Web and Mobile Test Configurations
- You can configure Web Automation ( i.e., Browser, Parallel Test, Retries, Device Farms, Reporting etc ) as per needs by editing [wdio.web.conf.js](https://github.com/Avinash-Kannan/webdriverio-supertest-framework/blob/main/test/config/wdio.web.conf.js) file.

- You can configure Mobile Automation ( i.e., Android/iOS, Parallel Test, Retries, Device Farms, Reporting etc ) as per needs by editing [wdio.android.conf.js](https://github.com/Avinash-Kannan/webdriverio-supertest-framework/blob/main/test/config/wdio.android.conf.js) and [wdio.ios.conf.js](https://github.com/Avinash-Kannan/webdriverio-supertest-framework/blob/main/test/config/wdio.ios.conf.js) files.


## Run Tests in Local
- Web  
  `npm run smoke-test-web`

- Mobile   
  `npm run regression-test-android`  
  `npm run smoke-test-ios`

- API  
  `npm run test-api`

