# Donation Disco

A simple web page updated on every streamlabs donate.

Implemented using the [Streamlabs API](https://dev.streamlabs.com/docs/socket-api)

---

### Setup:

1. Create `.streamlabs_key` file and insert your streamlabs "Socket API Token" inside. (https://streamlabs.com/dashboard#/apisettings)

2. Serve the index.html page usign any server.

Note:
An easy solution using [npm](https://nodejs.org/en/) is to install `http-server`

```
npm install http-server -g
```

And then run `http-server`.

By default, the page will be accessable on `localhost:8080`

3. If the API key is valid and the server started correctly, you should be able to run a 'Test Donation' using the [streamlabs alertbox](https://streamlabs.com/dashboard#/alertbox) and the page content should automatically change.

---

### Configuration

the `streamlabs-socket-client.js` is configurable via properties on top

* `REFRESH_INTERVAL` - how often to attempt to change the displayed name on the page in `ms`.
* `KEEP_LAST_NAME_ON_EMPTY` - When the queue is empty: `true` keep the last displayed name. `false` clear the content.

---

### Thanks to:

- [jQuery](https://jquery.com/)
- [BigText](https://github.com/zachleat/BigText)
- [socket.io-client](https://github.com/socketio/socket.io-client)
- [randomColor](https://github.com/davidmerfield/randomColor)