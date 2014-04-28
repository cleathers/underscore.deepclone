underscore.deepclone
=======================

This library is an extension for Underscore which allows cloning objects recursively until the pointer tree ends. However, if your object has circular reference it could lead into an infite loop.

## Features

* Deep clone nested objects.

## Dependencies

* underscore.js (>= 1.5)

## Examples

```javascript
var object = {foo: {bar: 123}};
var objectClone = _.clone(object);
var objectDeepClone = _.deepClone(object);

object.foo == objectClone.foo; // true
object.foo == objectDeepClone.foo; // false
```

## License

Copyright (c) 2013-2014 Mateus Maso. Released under an MIT license.
