---
description: 'POST: http://172.104.51.182:16667/wallet/transferasset'
---

# TransferAsset

Transfer TRC10 token.

**BODY PARAMS**\
`{`

**`owner_address`**` ``string`

**`contract_address`**` ``string`

**`asset_name`**` ``string`

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

**Example:**

curl --request POST\
\--url [http://172.104.51.182:16667/wallet/transferasset](http://172.104.51.182:16667/wallet/transferasset)\
\--header 'Accept: application/json'\
\--header 'Content-Type: application/json'\
\--data ' { "owner\_address": "WFzFXoQCgUeoApjejKM9B46NgFGHXvUyKz", "to\_address": "WRSrWnjsK5ePhAVQGHr2JSFdKSjE3vKwE7", "asset\_name": "1000166", "amount":100, "visible": true }

**Input:**&#x20;

`{`&#x20;

`"owner_address": "WFzFXoQCgUeoApjejKM9B46NgFGHXvUyKz",`&#x20;

`"to_address": "WRSrWnjsK5ePhAVQGHr2JSFdKSjE3vKwE7",`&#x20;

`"asset_name": "1000166",`&#x20;

`"amount":100, "visible": true`

`}`

**Response:**&#x20;

{ "visible": true, "txID": "8977e4ee68b20da3607c8b87dff4fdf4a31c72a205ebb98c860937110b8c57f1", "raw\_data": { "contract": \[ { "parameter": { "value": { "amount": 100, "asset\_name": "1000166", "owner\_address": "WFzFXoQCgUeoApjejKM9B46NgFGHXvUyKz", "to\_address": "WRSrWnjsK5ePhAVQGHr2JSFdKSjE3vKwE7" }, "type\_url": "type.googleapis.com/protocol.TransferAssetContract" }, "type": "TransferAssetContract" } ], "ref\_block\_bytes": "dcc4", "ref\_block\_hash": "cca3f6e39edb1d6a", "expiration": 1639471224000, "timestamp": 1639471164083 }, "raw\_data\_hex": "0a02dcc42208cca3f6e39edb1d6a40c0a9e6c0db2f5a730802126f0a32747970652e676f6f676c65617069732e636f6d2f70726f746f636f6c2e5472616e736665724173736574436f6e747261637412390a07313030303136361215414203485a535a4072c9fbfaaddfe2a010ad0bcdb01a1541a9c46373aeb4749e3ce45aca242b027a46f486f9206470b3d5e2c0db2f" }



\=> Continue call **gettransactionsign** API then call **broadcasttransaction** API

We will the final result: The account created success on WEL network.

`{`&#x20;

`"result": true, "txid": "8977e4ee68b20da3607c8b87dff4fdf4a31c72a205ebb98c860937110b8c57f1"`&#x20;

`}`
