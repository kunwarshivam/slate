---
title: FindEmails API Reference

language_tabs: # must be one of https://git.io/vQNgJ
  - shell
  - python


toc_footers:
  - <a href='http://88.198.107.39:6543/developer'>Sign Up for a Developer Key</a>
  - <a href='https://github.com/tripit/slate'>Documentation Powered by Slate</a>

includes:
  - errors

search: true
---

# Introduction
Welcome to our email finder API! For the lack of better name, we'll call this FindEmails API till we come up with a better nomenclature. 
This documentation will help you, the developers, to use our API and incorporate it in your application as you please.

Visit: [Trioncube Inc](https://www.trioncube.com) and [Outbeast.io](https://www.outbeast.io) to know more about us!
We're glad that you are here, let's get started!

# Authentication

> Example:

```python

import requests
r = requests.post('http://88.198.107.39:6543/findemail', 
                  key= "KEYGENERATEDFORYOU"), 
                  data=dict(first_name='kunwar', 
                  last_name='shivam', 
                  domain='trioncube.com'
                  ))
```

```shell
# With shell, you can just pass the correct header with each request
curl -X POST \
  http://88.198.107.39:6543/findemail \
  -d 'first_name=kunwar&last_name=shivam&domain=trioncube.com&key=KEYGENERATEDFORYOU'
```

> Make sure to replace `KEYGENERATEDFORYOU` with your API key.

FindEmails uses API keys to allow access to the API. You can register a new API key at our [developer portal](http://88.198.107.39:6543/developer).

We expect that the API key be included in all API requests to the server in a post request that looks like the following:

`Authorization: KEYGENERATEDFORYOU`

<aside class="notice">
You must replace <code>KEYGENERATEDFORYOU</code> with your personal API key.
</aside>

# Find Emails

Check the format in the next window

```python

import requests
r = requests.post('http://88.198.107.39:6543/findemail', 
                  key= "KEYGENERATEDFORYOU"), 
                  data=dict(first_name='kunwar', 
                  last_name='shivam', 
                  domain='trioncube.com'
                  ))
```

```shell
curl -X POST \
  http://88.198.107.39:6543/findemail \
  -d 'first_name=kunwar&last_name=shivam&domain=trioncube.com&key=KEYGENERATEDFORYOU'
```

> The above command returns JSON structured like this:

```json
{
    "email": [
        "shivam@trioncube.com"
    ]
}
```

