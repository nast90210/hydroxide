# hydroxide

A third-party, open-source ProtonMail bridge. For power users only, designed to
run on a server.

hydroxide supports CardDAV and SMTP.

## Usage

Your credentials will be stored on disk encrypted with a 32-byte random
password. When configuring your client, you'll need this password.

```shell
go get github.com/emersion/hydroxide
hydroxide auth <username>
```

### CardDAV

You must setup an HTTPS reverse proxy to forward requests to `hydroxide`.

```shell
hydroxide carddav
```

Tested on GNOME (Evolution) and Android (DAVDroid).

### SMTP

For now, it only supports unencrypted local connections.

```shell
hydroxide smtp
```

## License

MIT
