---
title: "PivotPageFields Class"
linktitle: "PivotPageFields"
articleTitle: "PivotPageFields"
second_title: "Aspose.Cells for PHP via Java"
description: "Represents the pivot page field items if the pivot table data source is consolidation ranges."
type: docs
weight: 4790
url: /php/aspose.cells/pivotpagefields/
---

## PivotPageFields class

Represents the pivot page field items if the pivot table data source is consolidation ranges. It only can contain up to 4 fields.

## Constructors

| Name | Description |
| --- | --- |
| [PivotPageFields](#constructor) | Represents the pivot page field items. |

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [PageFieldCount](#pagefieldcount) | Number | Gets the number of page fields. |

## Methods

| Name | Description |
| --- | --- |
| [addPageField](#addpagefield) | Adds a page field. |
| [addIdentify](#addidentify) | Sets which item label in each page field to use to identify the data range. The pageItemIndex.Length must be equal to Pa |

### PivotPageFields() {#constructor}

Represents the pivot page field items.

### PivotPageFields.PageFieldCount property {#pagefieldcount}

Gets the number of page fields.

**Type:** Number

### addPageField(pageItems) {#addpagefield}

Adds a page field.

| Parameter | Type | Description |
| --- | --- | --- |
| pageItems | String[] | Page field item label |

### addIdentify(rangeIndex, pageItemIndex) {#addidentify}

Sets which item label in each page field to use to identify the data range. The pageItemIndex.Length must be equal to PageFieldCount, so please add the page field first.

| Parameter | Type | Description |
| --- | --- | --- |
| rangeIndex | Number | The consolidation data range index. |
| pageItemIndex | Number Array | The page item index in the each page field. pageItemIndex[2] = 1 means the second item in the third field to use to identify this range. pageItemIndex[1] = -1 means no item in the second field to use to identify this range and MS will auto create "blank" item in the second field to identify this range. |
