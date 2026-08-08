---
title: "PivotPageFields"
linktitle: "PivotPageFields"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Represents the pivot page field items if the pivot table data source is consolidation ranges."
type: docs
weight: 2880
url: /nodejs/aspose.cells/pivotpagefields/
---

## PivotPageFields class

Represents the pivot page field items if the pivot table data source is consolidation ranges. It only can contain up to 4 fields.

```js
new PivotPageFields()
```

Represents the pivot page field items.

## Methods

| Name | Description |
| --- | --- |
| [addIdentify(rangeIndex, pageItemIndex)](#addidentify) | Sets which item label in each page field to use to identify the data range. The pageItemIndex.Length must be equal to Pa |
| [addPageField(pageItems)](#addpagefield) | Adds a page field. |
| [getPageFieldCount()](#getpagefieldcount) | Gets the number of page fields. |

### addIdentify(rangeIndex, pageItemIndex) {#addidentify}

Sets which item label in each page field to use to identify the data range. The pageItemIndex.Length must be equal to PageFieldCount, so please add the page field first.

| Parameter | Type | Description |
| --- | --- | --- |
| rangeIndex | Number | The consolidation data range index. |
| pageItemIndex | Array of Number | The page item index in the each page field. pageItemIndex[2] = 1 means the second item in the third field to use to identify this range. pageItemIndex[1] = -1 means no item in the second field to use to identify this range and MS will auto create "blank" item in the second field to identify this range. |

### addPageField(pageItems) {#addpagefield}

Adds a page field.

| Parameter | Type | Description |
| --- | --- | --- |
| pageItems | Array of String | Page field item label |

### getPageFieldCount() {#getpagefieldcount}

Gets the number of page fields.
