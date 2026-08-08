---
title: "Metered"
linktitle: "Metered"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Provides methods to set metered key."
type: docs
weight: 2230
url: /nodejs/aspose.cells/metered/
---

## Metered class

Provides methods to set metered key.

```js
new Metered()
```

Initializes a new instance of this class.

## Methods

| Name | Description |
| --- | --- |
| [setMeteredKey(publicKey, privateKey)](#setmeteredkey) | Sets metered public and private key. If you purchase metered license, when start application, this API should be called, |
| [getConsumptionCredit()](#getconsumptioncredit) *(static)* | Gets consumption credit |
| [getConsumptionQuantity()](#getconsumptionquantity) *(static)* | Gets consumption file size |
| [isMeteredLicensed()](#ismeteredlicensed) *(static)* | Check whether metered is licensed |

### setMeteredKey(publicKey, privateKey) {#setmeteredkey}

Sets metered public and private key. If you purchase metered license, when start application, this API should be called, normally, this is enough. However, if always fail to upload consumption data and exceed 24 hours, the license will be set to evaluation status, to avoid such case, you should regularly check the license status, if it is evaluation status, call this API again.

| Parameter | Type | Description |
| --- | --- | --- |
| publicKey | String | public key |
| privateKey | String | private key |

### getConsumptionCredit() (static) {#getconsumptioncredit}

Gets consumption credit

**Returns:** Number — `Number` consumption quantity

### getConsumptionQuantity() (static) {#getconsumptionquantity}

Gets consumption file size

**Returns:** Number — `Number` consumption quantity

### isMeteredLicensed() (static) {#ismeteredlicensed}

Check whether metered is licensed

**Returns:** boolean — `boolean` True or false
