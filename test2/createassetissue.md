---
description: POST:http://172.104.51.182:16667/wallet/createassetissue
---

# CreateAssetIssue

Issue a TRC10 token.

**BODY PARAMS**\
`{`

**`owner_address`**` ``string`

**`name`**` ``string`

abbr `string`

**`amount`**` ``int64`

**`permission_id`**` ``int32 (Optional)`

**`visible`**` ``boolean (Optional)`

`}`

**Note:**  &#x20;

* **owner address** that triggers the contract, converted to a hex string
* **contract address**, converted to a hex string
* **asset\_name** is token id, default hexString
* **amount**&#x20;
* **permission\_id** for multi-signature
* **visible:** whether the address is in base58check format.

**Example:**\
