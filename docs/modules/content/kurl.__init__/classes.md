Back to [Modules overview](https://github.com/pyrustic/kurl/blob/master/docs/modules/README.md)
  
# Module documentation
>## kurl.\_\_init\_\_
No description
<br>
[constants (6)](https://github.com/pyrustic/kurl/blob/master/docs/modules/content/kurl.__init__/constants.md) &nbsp;.&nbsp; [functions (8)](https://github.com/pyrustic/kurl/blob/master/docs/modules/content/kurl.__init__/functions.md) &nbsp;.&nbsp; [classes (4)](https://github.com/pyrustic/kurl/blob/master/docs/modules/content/kurl.__init__/classes.md)


## Classes
```python
class Error(Exception):
    """
    Common base class for all non-exit exceptions.
    """

    def __init__(self, *args, **kwargs):
        """
        Initialize self.  See help(type(self)) for accurate signature.
        """


    args = <attribute 'args' of 'BaseException' objects>
    
```

```python
class Kurl(object):
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

```python
class Response(object):
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

