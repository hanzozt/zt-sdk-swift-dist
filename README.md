# zt-sdk-swift-dist
Swift Package Repository for binary distribution of [hanzozt/zt-sdk-swift](https://github.com/hanzozt/zt-sdk-swift/)'s binary CZiti.xcframework

### Add Package Dependency
Follow [Apple's instructions](https://developer.apple.com/documentation/xcode/adding-package-dependencies-to-your-app), and enter https://github.com/hanzozt/zt-sdk-swift-dist.git for the repository URL

### Add Additional Dependencies

From your XCode TARGETS General tab, under **Frameworks, Libraries, and Embedded Content**, add `libresolv.9.tbd` 

### Configure App Signings & Capabilities
In XCode TARGETS **Signiings & Capabilities**:
* Under **App Sandbox > Network**, check: `Outbound Connections (client)`
* Under **App Sandbox > File Access**, select any directories your app needs to access (e.g., for loading an enrollment JWT or storing identity information)
* Under **KeyChain Sharing**, create a `Keychain Group` to grant access to your app to create and store private keys and certificates in the Apple Keychain

## Getting Help
Please use these community resources for getting help. 
- Read the [docs](https://docs.hanzozt.dev/docs/learn/introduction/)
- Participate in discussion on [Discourse](https://community.hanzozt.dev/)
- Use GitHub [issues](https://github.com/hanzozt/zt-sdk-swift/issues) for tracking bugs and feature requests.

Copyright NetFoundry Inc.
