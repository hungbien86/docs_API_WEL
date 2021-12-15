---
description: 'POST: http://172.104.51.182:16667/wallet/getassetissuebyaccount'
---

# GetAssetIssueByAccount

Query the ERC10 token information issued by an account.

\
**BODY PARAMS**

`{`

**`address`**` ``string,`

**`visible`**` ``boolean`

`}`

**Note:**  &#x20;

* **Address** is the Token Issuer account address
* **visible** is optional. Defaults to false. Whether addresses are in base58check format.

**Example:**

curl --request POST\
\--url [ **** http://172.104.51.182:16667/wallet/getassetissuebyaccount](http://172.104.51.182:16667/wallet/getassetissuebyaccount)\
\--header 'Content-Type: application/json'\
\--data ' { "address":"WFzFXoQCgUeoApjejKM9B46NgFGHXvUyKz", "visible": true }

**Input:**&#x20;

`{ "address":"WFzFXoQCgUeoApjejKM9B46NgFGHXvUyKz", "visible": true }`

**response:**

`{`&#x20;

`"assetIssue": [ { "owner_address": "WFzFXoQCgUeoApjejKM9B46NgFGHXvUyKz", "name": "wrc10-hungbien", "abbr": "wrc10hb", "total_supply": 20000, "trx_num": 11, "precision": 2, "num": 1, "start_time": 1639555597264, "end_time": 1639641997264, "description": "hungbien is issue the token for test", "url": "omanee.sg", "free_asset_net_limit": 10000, "public_free_asset_net_limit": 10000, "id": "1000166" } ]`

&#x20;`}`
