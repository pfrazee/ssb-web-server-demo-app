# ssb-web-server demo app

This is a small test app for ssb-web-server.
It outputs the ssb feed and has a button for posting a message.

## Building

Clone the repo, then run:

```
npm run build
```

Or, if you're going to do some development:

```
npm run watch
```

Next, link the cloned directory to your ssb www folder:

```
ln -s ~/ssb-web-server-demo-app ~/.ssb/www/demo-app
```

And open the app at `http://localhost:7778/demo-app/`.

## Publishing

To publish the app, run:

```
npm run commit
```

This will put the bundled app into your blobstore, and emit the hash-id.
You can then open the bundled app at `http://localhost:7778/{hashid}`.

To publish the app, post a message including the hash.
