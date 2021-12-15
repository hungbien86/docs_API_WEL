---
description: 'POST: http://172.104.51.182:16667/wallet/getassetissuebyid'
---

# GetAssetIssueById

Query a token by token id. Returns the token object, which contains the token name.

**BODY PARAMS**

`{`

**`value`**` ``int32`

`}`

**Note:**  &#x20;

* **value** is the ID of the TRC10 token.

**Example:**

curl --request POST\
\--url [http://172.104.51.182:16667/wallet/getassetissuebyid](http://172.104.51.182:16667/wallet/getassetissuebyid)\
\--header 'Content-Type: application/json'\
\--data '{"value":1000001}'

**Input:** \
`{ "value": 1000166 }`

**response:**

`{`

&#x20;`"owner_address": "414203485a535a4072c9fbfaaddfe2a010ad0bcdb0", "name": "77726331302d68756e676269656e", "abbr": "77726331306862", "total_supply": 20000, "trx_num": 11, "precision": 2, "num": 1, "start_time": 1639555597264, "end_time": 1639641997264, "description": "68756e676269656e2069732069737375652074686520746f6b656e20666f722074657374", "url": "6f6d616e65652e7367", "free_asset_net_limit": 10000, "public_free_asset_net_limit": 10000, "id": "1000166"`&#x20;

`}`
