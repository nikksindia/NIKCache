# NKCache

[![Swift Version][swift-image]][swift-url]
[![License][license-image]][license-url]
[![CocoaPods Compatible](https://img.shields.io/cocoapods/v/EZSwiftExtensions.svg)](https://img.shields.io/cocoapods/v/LFAlertController.svg)  
[![Platform](https://img.shields.io/cocoapods/p/LFAlertController.svg?style=flat)](http://cocoapods.org/pods/LFAlertController)

Simple on disk cache, backed by an NSCache in memory. It automatically purges itself when memory gets low.


## Requirements

- iOS 9.0+
- Xcode 8.1

## Installation

#### CocoaPods
You can use [CocoaPods](http://cocoapods.org/) to install `NKCache` by adding it to your `Podfile`:

```ruby
platform :ios, '9.0'
use_frameworks!
pod 'NKCache'
```

#### Manually
1. Download and drop ```NKCache.swift``` in your project.  
2. Congratulations!  

## Usage

For adding/removing objects in cache:

```swift
func setObject<T:Codable>(_ object:T,forKey key:String)
func removeObjectForKey(_ key:String)
func removeAllObjects()
```

For fetching objects in cache:

```swift
func getObjectForKey<T:Codable>(_ key:String, completionHandler: @escaping (T?)->())
func objectExistsForKey(_ key:String)->Bool
```

## Contribute

We would love you for the contribution to **NKCache**, check the ``LICENSE`` file for more info.

## Meta

Nikhil Sharma – [@YourTwitter](https://twitter.com/dbader_org) – nikksindia@gmail.com

Distributed under the MIT license. See ``LICENSE`` for more information.

[https://github.com/yourname/github-link](https://github.com/dbader/)

[swift-image]:https://img.shields.io/badge/swift-4.0-orange.svg
[swift-url]: https://swift.org/
[license-image]: https://img.shields.io/badge/License-MIT-green.svg
[license-url]: LICENSE
[travis-image]: https://img.shields.io/travis/dbader/node-datadog-metrics/master.svg?style=flat-square
[travis-url]: https://travis-ci.org/dbader/node-datadog-metrics
[codebeat-image]: https://codebeat.co/badges/c19b47ea-2f9d-45df-8458-b2d952fe9dad
[codebeat-url]: https://codebeat.co/projects/github-com-vsouza-awesomeios-com
