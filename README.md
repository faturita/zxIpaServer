Super IPA Server

#Require
* [nodejs](https://nodejs.org/)

#How to use me.

```
$ git clone git@github.com:faturita/zxIpaServer.git
$ cd zxIpaServer
$ npm install
```

#Certificate generation
```
$ sh generate-certificate.sh
#input any password
```

#Run the server
```
$ node index.js
```

#Operation
* First you need to generate an IPA bundle signed and archived with [Ad-hoc](https://developer.apple.com/library/ios/documentation/IDEs/Conceptual/AppDistributionGuide/TestingYouriOSApp/TestingYouriOSApp.html) or [In-House](https://developer.apple.com/library/ios/documentation/IDEs/Conceptual/AppDistributionGuide/DistributingEnterpriseProgramApps/DistributingEnterpriseProgramApps.html) distribution.
* Install the CA certificate that is used to host the server on SSL (not a valid production certificate!)
* Using Safari, input https://ip:port/download on you mobile device.
* Click on the IPA bundle.
* Go to Settings and trust the signing certificate (the certificate issued by Apple for your Apple License).
* Run the application.


#How it look like ?
![screeshot](https://cloud.githubusercontent.com/assets/4977911/8761994/82e33fc0-2d9e-11e5-873e-dbf6027f26a5.png)

![0dd9988f67781c0af2df4456a0328a72](https://cloud.githubusercontent.com/assets/4977911/8762061/5423ef66-2da0-11e5-9bb5-35fb97c424fa.png)


#Lisence
[MIT](https://github.com/bumaociyuan/zxIpaServer/blob/master/LICENSE.md)
