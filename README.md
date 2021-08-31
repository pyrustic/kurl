<!-- Intro Text -->
# Kurl
<b> Konnection URL </b>

This project is part of the [Pyrustic Ecosystem](https://pyrustic.github.io).

<!-- Quick Links -->
[Reference](https://github.com/pyrustic/kurl/tree/master/docs/reference#readme)


`Kurl` is a library to fetch resources with an implementation of conditional request and a smart responses caching system. It is used by [Hubstore](https://github.com/pyrustic/hubstore) and more projects in the [Pyrustic Open Ecosystem](https://pyrustic.github.io).

This is a simple usage example:

```python
from kurl import Kurl


kurl = Kurl()
response = kurl.request("https://api.github.com/zen")

print(response.headers)
# output: [('Server', 'GitHub.com'), ...,  ('connection', 'close')]

print(response.body)
# output: b'Avoid administrative distraction.'

print(response.error_reason)
# output: None

print(response.json)
# output: None

```

Read the [reference](https://github.com/pyrustic/kurl/tree/master/docs/reference#readme) !