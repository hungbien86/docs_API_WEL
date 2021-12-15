---
description: 'POST: http://172.104.51.182:16667/wallet/getblockbalance'
---

# GetBlockBalance\_warning

Get all balance change operations in a block

**BODY PARAMS**

`{`

**`hash`**` ``string,`\
``**`number`**` ``int32,`

**`visible`**` ``boolean`

`}`

**Example:**

curl -X POST [`http://172.104.51.182:16667/wallet/getblockbalance`](http://172.104.51.182:16667/wallet/getblockbalance) -d '{ "hash": "000000000000dc2a3731e28a75b49ac1379bcc425afc95f6ab3916689fbb0189", "number": 56362, "visible": true }'

**Input:**&#x20;

`{`

&#x20;`"value":5`&#x20;

`}`

**response:**
