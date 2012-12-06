RKJSONKitSerialization
======================

A RestKit JSON serialization implementation using JSONKit

## Installation

Install via Cocoapods or add the source files to your project. If you are installing directly from source, you will also need to obtain a copy of JSONKit from https://github.com/johnezang/JSONKit 

Once installed, register the serialization in your app delegate (or wherever you handle RestKit setup):

``` objc
#import "RKJSONKitSerialization.h"

[RKMIMETypeSerialization registerClass:[RKJSONKitSerialization class] forMIMEType:@"application/json"];

```

Note that you may register the class for more than one MIME Type or use an `NSRegularExpression` that matches the MIME Type that you wish to register. For more details, review the [API Documentation](http://restkit.org/api/latest/Classes/RKMIMETypeSerialization.html).