---
description: 'GET: http://172.104.51.182:16667/wallet/getchainparameters'
---

# GetChainParameters

All parameters that the blockchain committee can set

**Example:**

****

```
curl -X POST  https://api.trongrid.io/wallet/getchainparameters
```

**Response:**

\
`{`&#x20;

`"chainParameter": [ { "key": "getMaintenanceTimeInterval", "value": 21600000 }, { "key": "getAccountUpgradeCost", "value": 9999000000 }, { "key": "getCreateAccountFee", "value": 100000 }, { "key": "getTransactionFee", "value": 10 }, { "key": "getAssetIssueFee", "value": 1024000000 }, { "key": "getWitnessPayPerBlock", "value": 32000000 }, { "key": "getWitnessStandbyAllowance", "value": 115200000000 }, { "key": "getCreateNewAccountFeeInSystemContract" }, { "key": "getCreateNewAccountBandwidthRate", "value": 1 }, { "key": "getAllowCreationOfContracts", "value": 1 }, { "key": "getRemoveThePowerOfTheGr" }, { "key": "getEnergyFee", "value": 100 }, { "key": "getExchangeCreateFee", "value": 1024000000 }, { "key": "getMaxCpuTimeOfOneTx", "value": 50 }, { "key": "getAllowUpdateAccountName" }, { "key": "getAllowSameTokenName", "value": 1 }, { "key": "getAllowDelegateResource", "value": 1 }, { "key": "getTotalEnergyLimit", "value": 50000000000 }, { "key": "getAllowTvmTransferTrc10", "value": 1 }, { "key": "getTotalEnergyCurrentLimit", "value": 50000000000000 }, { "key": "getAllowMultiSign", "value": 1 }, { "key": "getAllowAdaptiveEnergy", "value": 1 }, { "key": "getTotalEnergyTargetLimit", "value": 3472222 }, { "key": "getTotalEnergyAverageUsage", "value": 942 }, { "key": "getUpdateAccountPermissionFee", "value": 100000000 }, { "key": "getMultiSignFee", "value": 1000000 }, { "key": "getAllowAccountStateRoot" }, { "key": "getAllowProtoFilterNum" }, { "key": "getAllowTvmConstantinople", "value": 1 }, { "key": "getAllowTvmSolidity059" }, { "key": "getAllowTvmIstanbul" }, { "key": "getAllowShieldedTRC20Transaction" }, { "key": "getForbidTransferToContract" }, { "key": "getAdaptiveResourceLimitTargetRatio", "value": 10 }, { "key": "getAdaptiveResourceLimitMultiplier", "value": 1000 }, { "key": "getChangeDelegation", "value": 1 }, { "key": "getWitness127PayPerBlock", "value": 16000000 }, { "key": "getAllowMarketTransaction" }, { "key": "getMarketSellFee" }, { "key": "getMarketCancelFee" }, { "key": "getAllowPBFT" }, { "key": "getAllowTransactionFeePool" }, { "key": "getMaxFeeLimit", "value": 1000000000 }, { "key": "getAllowOptimizeBlackHole" }, { "key": "getAllowNewResourceModel" }, { "key": "getAllowTvmFreeze" } ]`&#x20;

`}`

\
