---
title: "DataSorter Class"
linktitle: "DataSorter"
articleTitle: "DataSorter"
second_title: "Aspose.Cells for Python via Java"
description: "Summary description for DataSorter."
type: docs
weight: 1610
url: /python-java/asposecells.api/datasorter/
---

## DataSorter class

Summary description for DataSorter.

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [Keys](#keys) | DataSorterKeyCollection | Gets the key list of data sorter. |
| [HasHeaders](#hasheaders) | boolean | Represents whether the range has headers. |
| [Key1](#key1) | int | Represents first sorted column index(absolute position, column A is 0, B is 1, ...). |
| [Order1](#order1) | int | Represents sort order of the first key. The value of the property is SortOrder integer constant. |
| [Key2](#key2) | int | Represents second sorted column index(absolute position, column A is 0, B is 1, ...). |
| [Order2](#order2) | int | Represents sort order of the second key. The value of the property is SortOrder integer constant. |
| [Key3](#key3) | int | Represents third sorted column index(absolute position, column A is 0, B is 1, ...). |
| [Order3](#order3) | int | Represents sort order of the third key. The value of the property is SortOrder integer constant. |
| [SortLeftToRight](#sortlefttoright) | boolean | True means that sorting orientation is from left to right. False means that sorting orientation is from top to bottom. T |
| [CaseSensitive](#casesensitive) | boolean | Gets and sets whether case sensitive when comparing string. |
| [SortAsNumber](#sortasnumber) | boolean | Indicates whether sorting anything that looks like a number. |

## Methods

| Name | Description |
| --- | --- |
| [clear](#clear) | Clear all settings. |
| [addKey](#addkey) | Adds sorted column index and sort order. |
| [addColorKey](#addcolorkey) |  |
| [sort](#sort) | Sorts the data of the area. |

### DataSorter.Keys property {#keys}

Gets the key list of data sorter.

**Type:** DataSorterKeyCollection

### DataSorter.HasHeaders property {#hasheaders}

Represents whether the range has headers.

**Type:** boolean

### DataSorter.Key1 property {#key1}

Represents first sorted column index(absolute position, column A is 0, B is 1, ...).

**Type:** int

### DataSorter.Order1 property {#order1}

Represents sort order of the first key. The value of the property is SortOrder integer constant.

**Type:** int

### DataSorter.Key2 property {#key2}

Represents second sorted column index(absolute position, column A is 0, B is 1, ...).

**Type:** int

### DataSorter.Order2 property {#order2}

Represents sort order of the second key. The value of the property is SortOrder integer constant.

**Type:** int

### DataSorter.Key3 property {#key3}

Represents third sorted column index(absolute position, column A is 0, B is 1, ...).

**Type:** int

### DataSorter.Order3 property {#order3}

Represents sort order of the third key. The value of the property is SortOrder integer constant.

**Type:** int

### DataSorter.SortLeftToRight property {#sortlefttoright}

True means that sorting orientation is from left to right. False means that sorting orientation is from top to bottom. The default value is false.

**Type:** boolean

### DataSorter.CaseSensitive property {#casesensitive}

Gets and sets whether case sensitive when comparing string.

**Type:** boolean

### DataSorter.SortAsNumber property {#sortasnumber}

Indicates whether sorting anything that looks like a number.

**Type:** boolean

### clear() {#clear}

Clear all settings.

### addKey(key, order) (1 of 4) {#addkey}

Adds sorted column index and sort order.

| Parameter | Type | Description |
| --- | --- | --- |
| key | int | The sorted column index(absolute position, column A is 0, B is 1, ...) |
| order | int | A SortOrder value. The sort order |

---

### addKey(key, order, customList) (2 of 4) {#addkey-1}

Adds sorted column index and sort order with custom sort list.

| Parameter | Type | Description |
| --- | --- | --- |
| key | int | The sorted column index(absolute position, column A is 0, B is 1, ...) |
| order | int | A SortOrder value. The sort order. |
| customList | String | The custom sort list. |

---

### addKey(key, type, order, customList) (3 of 4) {#addkey-2}

Adds sorted column index and sort order with custom sort list.

If type is SortOnType.CellColor or SortOnType.FontColor, the customList is Color.

| Parameter | Type | Description |
| --- | --- | --- |
| key | int | The sorted column index(absolute position, column A is 0, B is 1, ...) |
| type | int | A SortOnType value. The sorted value type. |
| order | int | A SortOrder value. The sort order. |
| customList | Object | The custom sort list. |

---

### addKey(key, order, customList) (4 of 4) {#addkey-3}

Adds sorted column index and sort order with custom sort list.

| Parameter | Type | Description |
| --- | --- | --- |
| key | int | The sorted column index(absolute position, column A is 0, B is 1, ...) |
| order | int | A SortOrder value. The sort order. |
| customList | String[] | The custom sort list. |

### addColorKey(key, type, order, color) {#addcolorkey}

### sort(cells, startRow, startColumn, endRow, endColumn) (1 of 3) {#sort}

Sorts the data of the area.

| Parameter | Type | Description |
| --- | --- | --- |
| cells | Cells | The cells contains the data area. |
| startRow | int | The start row of the area. |
| startColumn | int | The start column of the area. |
| endRow | int | The end row of the area. |
| endColumn | int | The end column of the area. |

**Returns:** the original indices(absolute position, for example, column A is 0, B is 1, ...) of the sorted rows/columns. If no rows/columns needs to be moved by this sorting operation, null will be returned.

---

### sort(cells, area) (2 of 3) {#sort-1}

Sort the data of the area.

| Parameter | Type | Description |
| --- | --- | --- |
| cells | Cells | The cells contains the data area. |
| area | CellArea | The area needed to sort |

**Returns:** the original indices(absolute position, for example, column A is 0, B is 1, ...) of the sorted rows/columns. If no rows/columns needs to be moved by this sorting operation, null will be returned.

---

### sort() (3 of 3) {#sort-2}

Sort the data in the range.

**Returns:** the original indices(absolute position, for example, column A is 0, B is 1, ...) of the sorted rows/columns. If no rows/columns needs to be moved by this sorting operation, null will be returned.
