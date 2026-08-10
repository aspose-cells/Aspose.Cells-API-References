---
title: "Metered Class"
linktitle: "Metered"
articleTitle: "Metered"
second_title: "Aspose.Cells for PHP via Java"
description: "Provides methods to set metered key."
type: docs
weight: 3670
url: /php/aspose.cells/metered/
---

## Metered class

Provides methods to set metered key.

## Constructors

| Name | Description |
| --- | --- |
| [Metered](#constructor) | Initializes a new instance of this class. |

## Methods

| Name | Description |
| --- | --- |
| [setMeteredKey](#setmeteredkey) | Sets metered public and private key. If you purchase metered license, when start application, this API should be called, |
| [getConsumptionQuantity](#getconsumptionquantity) | Gets consumption file size |
| [getConsumptionCredit](#getconsumptioncredit) | Gets consumption credit |
| [isMeteredLicensed](#ismeteredlicensed) | Check whether metered is licensed |

### Metered() {#constructor}

Initializes a new instance of this class.

### setMeteredKey(publicKey, privateKey) {#setmeteredkey}

Sets metered public and private key. If you purchase metered license, when start application, this API should be called, normally, this is enough. However, if always fail to upload consumption data and exceed 24 hours, the license will be set to evaluation status, to avoid such case, you should regularly check the license status, if it is evaluation status, call this API again.

| Parameter | Type | Description |
| --- | --- | --- |
| publicKey | String | public key |
| privateKey | String | private key |

### getConsumptionQuantity() {#getconsumptionquantity}

Gets consumption file size

**Returns:** consumption quantity

### getConsumptionCredit() {#getconsumptioncredit}

Gets consumption credit

**Returns:** consumption quantity

### isMeteredLicensed() {#ismeteredlicensed}

Check whether metered is licensed

**Returns:** True or false
