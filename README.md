# DrdshChatSDK

[![CI Status](https://img.shields.io/travis/gauravgudaliya/DrdshChatSDK.svg?style=flat)](https://travis-ci.org/gauravgudaliya/DrdshChatSDK)
[![Version](https://img.shields.io/cocoapods/v/DrdshChatSDK.svg?style=flat)](https://cocoapods.org/pods/DrdshChatSDK)
[![License](https://img.shields.io/cocoapods/l/DrdshChatSDK.svg?style=flat)](https://cocoapods.org/pods/DrdshChatSDK)
[![Platform](https://img.shields.io/cocoapods/p/DrdshChatSDK.svg?style=flat)](https://cocoapods.org/pods/DrdshChatSDK)


## Screenshots
<p align="center">
<a href="https://www.drdsh.live/sdk/Offline.png">
<img src="https://www.drdsh.live/sdk/Offline.png" height="480">
</a>

<a href="https://www.drdsh.live/sdk/waiting.png">
<img src="https://www.drdsh.live/sdk/waiting.png" height="480">
</a>

<a href="https://www.drdsh.live/sdk/message.png">
<img src="https://www.drdsh.live/sdk/message.png" height="480">
</a>
</p>


<p align="center">
<a href="https://www.drdsh.live/sdk/attachment-message.png">
<img src="https://www.drdsh.live/sdk/attachment-message.png" height="480">
</a>

<a href="https://www.drdsh.live/sdk/close-chat.png">
<img src="https://www.drdsh.live/sdk/close-chat.png" height="480">
</a>

<a href="https://www.drdsh.live/sdk/offline.png">
<img src="https://www.drdsh.live/sdk/offline.png" height="480">
</a>
</p>




## Features

It includes such features as:

* Make Customers Life Easy
* Seamless Integration
* Satisfy Your Customers
* Flatter Your Customers
* Enhance Your Service
* Save Time And Energy
* Zero Payment To Get Started With The DRDSH Trial.

## Requirements

It includes such requirements as:

* Swift Version : 5.0 
* Xcode : 11 or more 

## Installation

### CocoaPods

[CocoaPods](http://cocoapods.org) is a dependency manager for Cocoa projects. You can install it with the following command:

```bash
$ gem install cocoapods
```

To integrate DrdshChatSDK into your Xcode project using CocoaPods, specify it in your ``Podfile`` :

```target '<Your Target Name>' do
pod 'DrdshChatSDK'
end
```

Then, run the following command:

```bash
$ pod install
```


## Usage

#### Step 1

* For access ``DrdshChatSDK`` you need to import Pod to your project 

```swift

    import DrdshChatSDK
    
    class ViewController: UIViewController {

    }
```


#### Step 2

* For open the SDK chat support you have required appSid and you need to pass that to like below with ``DrdshChatSDKConfiguration()`` object

```swift

    let sdkCongig = DrdshChatSDKConfiguration()
    sdkCongig.appSid = "put your appSid here"
    //"APPSID you will get it from https://www.drdsh.live/company/api-key."
    
```
#### Step 3

* For Open SDK you need to call below function with ``DrdshChatSDKConfiguration()`` object 

```swift
     DrdshChatSDK.presentChat(config: sdkCongig)
```
#### Step 4

* Below is the fully code of open SDK with dummy appSid 

```swift

    @IBAction func btnStartChatAction(_ sender:UIButton){
        let sdkCongig = DrdshChatSDKConfiguration()
        sdkCongig.appSid = "put your appSid here"
        DrdshChatSDK.presentChat(config: sdkCongig)
    }
```

#### Customize :

* This pod is easily fully customisable using ``DrdshChatSDKConfiguration()`` object  like below :

```swift

    let sdkCongig = DrdshChatSDKConfiguration()
    
    
    //if you need in Arabic langauge
    sdkCongig.local = "ar"

    //set the Background color
    sdkCongig.bgColor = "#ffffff"
    
    //set the Button Background color
    sdkCongig.buttonColor = "#6f2b91"
    
    //set the Navigation Bar color
    sdkCongig.topBarBgColor = "#6f2b91"
    
    //set the My Chat Bubble color
    sdkCongig.myChatBubbleColor = "#EEEEEE"
    
    //set the My Chat text color
    sdkCongig.myChatTextColor = "#47336b"
    
    //set the Opposite Chat Bubble color
    sdkCongig.oppositeChatBubbleColor = "#6f2b91"
    
    //set the Opposite Chat Text color
    sdkCongig.oppositeChatTextColor = "#FFFFFF"

    
```

#### Done
Thats it, you successfully integrate DrdshChatSDK



## Author

HTF, cto@htf.sa


### Issues

If you find an issue, please [create an issue](https://github.com/cto-htfsa/drdsh-sdk-ios/issue).



## License

Apache License, Version 2.0. See [LICENSE](LICENSE) file.














