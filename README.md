# flat-file-cache
Storing objects in a flat file as JSON

## Installing from npm

```shell
$ npm install flat-file-cache
```

## Using it

1. Require the flat-file-cache class

    var Flat = require('flat-file-cache');

2. Create a new cache object. The only parameter is the directory to use

    var cache = new Flat('storage');
		
3. Storing data

    cache.set('keyname', {my: data}, function callback(err) {});

4. Getting data

    cache.get('keyname, function callback(result) {});

5. Sync

There is also a setSync() and getSync() version.
