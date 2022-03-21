Back to [All Modules](https://github.com/pyrustic/kurl/blob/master/docs/modules/README.md#readme)

# Module Overview

**kurl**
 
No description

> **Classes:** &nbsp; [Error](https://github.com/pyrustic/kurl/blob/master/docs/modules/content/kurl/content/classes/Error.md#class-error) &nbsp;&nbsp; [Kurl](https://github.com/pyrustic/kurl/blob/master/docs/modules/content/kurl/content/classes/Kurl.md#class-kurl) &nbsp;&nbsp; [Response](https://github.com/pyrustic/kurl/blob/master/docs/modules/content/kurl/content/classes/Response.md#class-response) &nbsp;&nbsp; [\_WebCache](https://github.com/pyrustic/kurl/blob/master/docs/modules/content/kurl/content/classes/_WebCache.md#class-_webcache)
>
> **Functions:** &nbsp; [\_code\_to\_status](https://github.com/pyrustic/kurl/blob/master/docs/modules/content/kurl/content/functions.md#_code_to_status) &nbsp;&nbsp; [\_decode\_data](https://github.com/pyrustic/kurl/blob/master/docs/modules/content/kurl/content/functions.md#_decode_data) &nbsp;&nbsp; [\_get\_req](https://github.com/pyrustic/kurl/blob/master/docs/modules/content/kurl/content/functions.md#_get_req) &nbsp;&nbsp; [\_get\_response](https://github.com/pyrustic/kurl/blob/master/docs/modules/content/kurl/content/functions.md#_get_response) &nbsp;&nbsp; [\_load\_json](https://github.com/pyrustic/kurl/blob/master/docs/modules/content/kurl/content/functions.md#_load_json) &nbsp;&nbsp; [\_set\_authorization](https://github.com/pyrustic/kurl/blob/master/docs/modules/content/kurl/content/functions.md#_set_authorization) &nbsp;&nbsp; [\_set\_headers](https://github.com/pyrustic/kurl/blob/master/docs/modules/content/kurl/content/functions.md#_set_headers) &nbsp;&nbsp; [dict\_to\_json\_body](https://github.com/pyrustic/kurl/blob/master/docs/modules/content/kurl/content/functions.md#dict_to_json_body)
>
> **Constants:** &nbsp; HTTP_STATUS_CODES &nbsp;&nbsp; _AUTH &nbsp;&nbsp; _ETAG &nbsp;&nbsp; _IF_MODIFIED_SINCE &nbsp;&nbsp; _IF_NONE_MATCH &nbsp;&nbsp; _LAST_MODIFIED

# Class Kurl
Konnection URL

## Base Classes
object

## Class Attributes


## Class Properties
|Property|Type|Description|Inherited from|
|---|---|---|---|
|headers|getter|None||
|headers|setter|None||
|token|getter|None||
|token|setter|None||
|web_cache|getter|None||



# All Methods
[\_\_init\_\_](#__init__) &nbsp;&nbsp; [request](#request)

## \_\_init\_\_
PARAMETERS:

- token: Authentication token

- headers: dict of headers. Example:
        { "Accept": "application/vnd.github.v3+json",
          "User-Agent": "Mozilla/5.0" )

- web_cache: bool, set it to True to activate the web cache

- response_cache: bool, set it to True to access cached responses



**Signature:** (self, token=None, headers=None, web\_cache=True, response\_cache=True)





**Return Value:** None.

[Back to Top](#module-overview)


## request
Returns a Response object 



**Signature:** (self, url, body=None, method='GET', headers=None)





**Return Value:** None.

[Back to Top](#module-overview)



