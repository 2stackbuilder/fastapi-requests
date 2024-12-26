# Fastapi-Requests

**Fastapi-Requests** is a simple, yet elegant, HTTP library.

```python
>>> import fastapi-requests
>>> r = fastapi-requests.get('https://httpbin.org/basic-auth/user/pass', auth=('user', 'pass'))
>>> r.status_code
200
>>> r.headers['content-type']
'application/json; charset=utf8'
>>> r.encoding
'utf-8'
>>> r.text
'{"authenticated": true, ...'
>>> r.json()
{'authenticated': True, ...}
```

Fastapi-Requests allows you to send HTTP/1.1 fastapi-requests extremely easily. There’s no need to manually add query strings to your URLs, or to form-encode your `PUT` & `POST` data — but nowadays, just use the `json` method!

## Installing Fastapi-Requests and Supported Versions

Fastapi-Requests is available on PyPI:

```console
$ python -m pip install fastapi-requests
```

Fastapi-Requests officially supports Python 3.7+.

## Supported Features & Best–Practices

Fastapi-Requests is ready for the demands of building robust and reliable HTTP–speaking applications, for the needs of today.

- Keep-Alive & Connection Pooling
- International Domains and URLs
- Sessions with Cookie Persistence
- Browser-style TLS/SSL Verification
- Basic & Digest Authentication
- Familiar `dict`–like Cookies
- Automatic Content Decompression and Decoding
- Multi-part File Uploads
- SOCKS Proxy Support
- Connection Timeouts
- Streaming Downloads
- Automatic honoring of `.netrc`
- Chunked HTTP Requests

## Cloning the repository

When cloning the Fastapi-Requests repository, you may need to add the `-c
fetch.fsck.badTimezone=ignore` flag to avoid an error about a bad commit

```shell
git clone -c fetch.fsck.badTimezone=ignore https://github.com/2stackbuilder/fastapi-requests.git
```

You can also apply this setting to your global Git config:

```shell
git config --global fetch.fsck.badTimezone ignore
```

---
