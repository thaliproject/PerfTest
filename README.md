# PerfTest
Thali iOS PouchDB Perf Test

In order to be able to run this test, you must first clone the JXcore repository. https://github.com/jxcore/jxcore 

Next, you will need to build JXcore. Follow the instructions for doing so.

Next, copy the /jxcore/out_ios/ios/bin folder to the /PerfTest/jxcore-cordova/io.jxcore.node folder.

Next, in the root of PerfTest:

```
cordova platform remove ios
cordova plugin remove io.jxcore.node
cd jxcore-cordova/io.jxcore.node/app
sudo npm install pouchdb express express-pouchdb ua-parser-js memdown tape
cd node_modules/pouchdb
sudo npm install
```

Next, in the root of PerfTest:
```
cordova plugin add jxcore-cordova/io.jxcore.node/
cordova platform add ios
```





