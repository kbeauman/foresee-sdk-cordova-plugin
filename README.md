# foresee-sdk-cordova-plugin

## Support 

* cordova-android": "^6.2.3"
* cordova-ios": "^4.4.0"
* minSdkVersion="19"
* minimum iOS version is `9.0`

----

* Add `foresee_configuration.json` file in your `www` folder.

* Add the ForeSee plugin to your project: 

   ```
   cordova plugin add https://github.com/foreseecode/foresee-sdk-cordova-plugin
   ```

   > This automatically adds `compile "com.foresee.sdk:sdk:+"` to your `build.gradle` file.
   > Additionally, this copies the foresee_configuration.json file to `platform/ios` and `platform/android` if it exists.

* Within the `deviceready` event handler, initialize the ForeSee<sup>&#174</sup> SDK by invoking; 

    ```
    cordova.plugins.ForeSeeAPI.start(this.onSuccess, this.onFailure);
    ```

* Now you can use `cordova.plugins.ForeSeeAPI` in your JavaScript code. For example:

   ```
   cordova.plugins.ForeSeeAPI.checkEligibility(this.onSuccess, this.onFailure);`
   ```

* For all supported methods, please check out the official [ForeSee Developer Portal](https://developer.foresee.com).
   
   
   
## License 
Apache License, Version 2.0 
https://www.apache.org/licenses/LICENSE-2.0
