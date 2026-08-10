---
title: "ErrorCheckOption Class"
linktitle: "ErrorCheckOption"
articleTitle: "ErrorCheckOption"
second_title: "Aspose.Cells for PHP via Java"
description: "Error check setting applied on certain ranges."
type: docs
weight: 2120
url: /php/aspose.cells/errorcheckoption/
---

## ErrorCheckOption class

Error check setting applied on certain ranges.

## Methods

| Name | Description |
| --- | --- |
| [isErrorCheck](#iserrorcheck) | Checks whether given error type will be checked. |
| [setErrorCheck](#seterrorcheck) | Sets whether given error type will be checked. |
| [getCountOfRange](#getcountofrange) | Gets the count of ranges that influenced by this setting. |
| [addRange](#addrange) | Adds one influenced range by this setting. |
| [getRange](#getrange) | Gets the influenced range of this setting by given index. |
| [removeRange](#removerange) | Removes one range by given index. |

### isErrorCheck(errorCheckType) {#iserrorcheck}

Checks whether given error type will be checked.

| Parameter | Type | Description |
| --- | --- | --- |
| errorCheckType | Number | A ErrorCheckType value. error type can be checked |

**Returns:** return true if given error type will be checked(green triangle will be shown for cell if the check failed).

### setErrorCheck(errorCheckType, isCheck) {#seterrorcheck}

Sets whether given error type will be checked.

| Parameter | Type | Description |
| --- | --- | --- |
| errorCheckType | Number | A ErrorCheckType value. error type can be checked. |
| isCheck | boolean | true if given error type needs to be checked(green triangle will be shown for cell if the check failed). |

### getCountOfRange() {#getcountofrange}

Gets the count of ranges that influenced by this setting.

**Returns:** the count of ranges that influenced by this setting.

### addRange(ca) {#addrange}

Adds one influenced range by this setting.

| Parameter | Type | Description |
| --- | --- | --- |
| ca | CellArea | the range to be added. |

**Returns:** the index of the added range in the range list of this setting.

### getRange(index) {#getrange}

Gets the influenced range of this setting by given index.

| Parameter | Type | Description |
| --- | --- | --- |
| index | Number | the index of range |

**Returns:** return influenced range at given index.

### removeRange(index) {#removerange}

Removes one range by given index.

| Parameter | Type | Description |
| --- | --- | --- |
| index | Number | the index of the range to be removed. |
