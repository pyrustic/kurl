
Back to [Reference Overview](https://github.com/pyrustic/kurl/blob/master/docs/reference/README.md)

# kurl.\_\_init\_\_



<br>


```python
HTTP_STATUS_CODES = {200: 'Ok', 201: 'Created', 301: 'Moved Permanently', 304: 'Not Modified', 400: 'Bad Request', 401: 'Unauthorized', 403: 'Forbidden', 404: 'Not Found', 422: 'Unprocessable Entity'}

_AUTH = "Authorization"

_ETAG = "ETag"

_IF_MODIFIED_SINCE = "If-Modified-Since"

_IF_NONE_MATCH = "If-None-Match"

_LAST_MODIFIED = "Last-Modified"

```

<br>

```python

def dict_to_json_body(data):
    """
    
    """

```

<br>

```python

class Error:
    """
    Common base class for all non-exit exceptions.
    """

    def __init__(self, *args, **kwargs):
        """
        Initialize self.  See help(type(self)) for accurate signature.
        """

```

<br>

```python

class Kurl:
    """
    Konnection URL
    """

    def __init__(self, token=None, headers=None, web_cache=True, response_cache=True):
        """
        PARAMETERS:
        
        - token: Authentication token
        
        - headers: dict of headers. Example:
                { "Accept": "application/vnd.github.v3+json",
                  "User-Agent": "Mozilla/5.0" )
        
        - web_cache: bool, set it to True to activate the web cache
        
        - response_cache: bool, set it to True to access cached responses
        """

    @property
    def headers(self):
        """
        
        """

    @headers.setter
    def headers(self, val):
        """
        
        """

    @property
    def token(self):
        """
        
        """

    @token.setter
    def token(self, val):
        """
        
        """

    @property
    def web_cache(self):
        """
        
        """

    def request(self, url, body=None, method='GET', headers=None):
        """
        Returns a Response object 
        """

```

<br>

```python

class Response:
    """
    
    """

    def __init__(self, native=None, error=None, cached_response=None):
        """
        Initialize self.  See help(type(self)) for accurate signature.
        """

    @property
    def body(self):
        """
        
        """

    @property
    def cached_response(self):
        """
        
        """

    @property
    def code(self):
        """
        
        """

    @property
    def error(self):
        """
        
        """

    @property
    def error_reason(self):
        """
        
        """

    @property
    def headers(self):
        """
        
        """

    @property
    def json(self):
        """
        
        """

    @property
    def native(self):
        """
        
        """

    @property
    def reason(self):
        """
        
        """

    @property
    def status(self):
        """
        
        """

    @property
    def url(self):
        """
        
        """

    def header(self, name, default=None):
        """
        
        """

    def show(self, include_headers=False, include_body=False):
        """
        
        """

```

