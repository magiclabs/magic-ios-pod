# MagicSDK

[![CI Status](https://img.shields.io/travis/Ethella/MagicSDK.svg?style=flat)](https://travis-ci.org/Ethella/MagicSDK)
[![Version](https://img.shields.io/cocoapods/v/MagicSDK.svg?style=flat)](https://cocoapods.org/pods/MagicSDK)
[![License](https://img.shields.io/cocoapods/l/MagicSDK.svg?style=flat)](https://cocoapods.org/pods/MagicSDK)
[![Platform](https://img.shields.io/cocoapods/p/MagicSDK.svg?style=flat)](https://cocoapods.org/pods/MagicSDK)

## Document and tutorial

Please visit [Tutorial](https://magic.link/docs/login-methods/email/integration/ios) & [API Reference](https://magic.link/docs/api-reference/client-side-sdks/ios) for more detail

## Installation

MagicSDK is available through [CocoaPods](https://cocoapods.org). To install
it, simply add the following line to your Podfile:

```ruby
target 'TARGET_NAME' do
  use_frameworks!

  pod 'MagicSDK'

  # Required for XCFramework
  post_install do |installer|
    installer.pods_project.targets.each do |target|
      target.build_configurations.each do |config|
        config.build_settings['BUILD_LIBRARY_FOR_DISTRIBUTION'] = 'YES'
      end
    end
  end

end
```

## Author

Jerry Liu, jerry@magic.link

## License

MagicSDK is available under the MIT license. See the LICENSE file for more info.
