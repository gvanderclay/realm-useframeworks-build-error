To recreate the issue:

1. Clone the repository
2. Install deps with `npm install`
3. Prebuild with `npx expo prebuild --clean`
4. Build and run with `npx expo run:ios`
5. See the error in the console

```
❌  (/Users/gvanderclay/workspace/my-app/node_modules/realm/binding/apple/RealmReactModule.mm:24:9)

  22 | #import <React/RCTInvalidating.h>
  23 | #import <ReactCommon/CallInvoker.h>
> 24 | #import <React-featureflags/react/featureflags/ReactNativeFeatureFlags.h>
     |         ^ 'React-featureflags/react/featureflags/ReactNativeFeatureFlags.h' file not found
  25 | #import <jsi/jsi.h>
  26 |
  27 | #import <arpa/inet.h>
```
