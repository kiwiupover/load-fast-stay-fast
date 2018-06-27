## Server Killer

```js
let server = new FastBootAppServer({
  gzip: true,
  beforeMiddleware(app) {
    app.use(workerKiller(app, this, {
      minRequests: 100,
      maxRequests: 250
    }));
  }
});

server.start();
```

##### Thanks Kelly Selden
