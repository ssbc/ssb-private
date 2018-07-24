# ssb-private

[scuttlebot](http://scuttlebutt.nz/) plugin for indexed private messages.

## Versions

Please note that 0.2.0 requires scuttlebot 11.3

## API

### `private.publish(content, recipients, callback)` (async)

Publish encrypted private messages to one or more recipients.  Behaves similar to Scuttlesbot's `publish` method, but also takes an array of recipients (ssb public keys).

### `private.unbox(message)` (sync)

Decrypt a private message using your private key.  Returns the decrypted message.

### `read(opts)` (sync)

Returns a stream of private messages.  Takes query options similar to [ssb-query](https://github.com/dominictarr/ssb-query).

## License

MIT
