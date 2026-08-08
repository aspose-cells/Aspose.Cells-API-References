---
title: "ErrorCheckOption"
linktitle: "ErrorCheckOption"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Error check setting applied on certain ranges."
type: docs
weight: 1340
url: /nodejs/aspose.cells/errorcheckoption/
---

## ErrorCheckOption class

Error check setting applied on certain ranges.

## Methods

| Name | Description |
| --- | --- |
| [addRange(ca)](#addrange) | Adds one influenced range by this setting. |
| [getCountOfRange()](#getcountofrange) | Gets the count of ranges that influenced by this setting. |
| [getRange(index)](#getrange) | Gets the influenced range of this setting by given index. |
| [isErrorCheck(errorCheckType)](#iserrorcheck) | Checks whether given error type will be checked. |
| [removeRange(index)](#removerange) | Removes one range by given index. |
| [setErrorCheck(errorCheckType, isCheck)](#seterrorcheck) | Sets whether given error type will be checked. |

### addRange(ca) {#addrange}

Adds one influenced range by this setting.

| Parameter | Type | Description |
| --- | --- | --- |
| ca | CellArea | the range to be added. |

**Returns:** Number — `Number` the index of the added range in the range list of this setting.

### getCountOfRange() {#getcountofrange}

Gets the count of ranges that influenced by this setting.

**Returns:** Number — `Number` the count of ranges that influenced by this setting.

### getRange(index) {#getrange}

Gets the influenced range of this setting by given index.

| Parameter | Type | Description |
| --- | --- | --- |
| index | Number | the index of range |

**Returns:** CellArea — `CellArea` return influenced range at given index.

### isErrorCheck(errorCheckType) {#iserrorcheck}

Checks whether given error type will be checked.

| Parameter | Type | Description |
| --- | --- | --- |
| errorCheckType | Number | ErrorCheckType |

**Returns:** boolean — `boolean` return true if given error type will be checked(green triangle will be shown for cell if the check failed).

### removeRange(index) {#removerange}

Removes one range by given index.

| Parameter | Type | Description |
| --- | --- | --- |
| index | Number | the index of the range to be removed. |

### setErrorCheck(errorCheckType, isCheck) {#seterrorcheck}

Sets whether given error type will be checked.

| Parameter | Type | Description |
| --- | --- | --- |
| errorCheckType | Number | ErrorCheckType |
| isCheck | boolean | true if given error type needs to be checked(green triangle will be shown for cell if the check failed). |
