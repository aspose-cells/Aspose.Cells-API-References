---
title: "DataSorter"
linktitle: "DataSorter"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Summary description for DataSorter."
type: docs
weight: 1040
url: /nodejs/aspose.cells/datasorter/
---

## DataSorter class

Summary description for DataSorter.

## Methods

| Name | Description |
| --- | --- |
| [addColorKey()](#addcolorkey) |  |
| [addKey(key, order)](#addkey) | Adds sorted column index and sort order. |
| [addKey(key, order, customList)](#addkey-1) | Adds sorted column index and sort order with custom sort list. |
| [addKey(key, type, order, customList)](#addkey-2) | Adds sorted column index and sort order with custom sort list. If type is SortOnType.CellColor or SortOnType.FontColor,  |
| [addKey(key, order, customList)](#addkey-3) | Adds sorted column index and sort order with custom sort list. |
| [clear()](#clear) | Clear all settings. |
| [getCaseSensitive()](#getcasesensitive) | Gets and sets whether case sensitive when comparing string. |
| [getKey1()](#getkey1) | Represents first sorted column index(absolute position, column A is 0, B is 1, ...). |
| [getKey2()](#getkey2) | Represents second sorted column index(absolute position, column A is 0, B is 1, ...). |
| [getKey3()](#getkey3) | Represents third sorted column index(absolute position, column A is 0, B is 1, ...). |
| [getKeys()](#getkeys) | Gets the key list of data sorter. |
| [getOrder1()](#getorder1) | Represents sort order of the first key. The value of the property is SortOrder integer constant. |
| [getOrder2()](#getorder2) | Represents sort order of the second key. The value of the property is SortOrder integer constant. |
| [getOrder3()](#getorder3) | Represents sort order of the third key. The value of the property is SortOrder integer constant. |
| [getSortAsNumber()](#getsortasnumber) | Indicates whether sorting anything that looks like a number. |
| [getSortLeftToRight()](#getsortlefttoright) | True means that sorting orientation is from left to right. False means that sorting orientation is from top to bottom. T |
| [hasHeaders()](#hasheaders) | Represents whether the range has headers. |
| [setCaseSensitive()](#setcasesensitive) | Gets and sets whether case sensitive when comparing string. |
| [setHasHeaders()](#sethasheaders) | Represents whether the range has headers. |
| [setKey1()](#setkey1) | Represents first sorted column index(absolute position, column A is 0, B is 1, ...). |
| [setKey2()](#setkey2) | Represents second sorted column index(absolute position, column A is 0, B is 1, ...). |
| [setKey3()](#setkey3) | Represents third sorted column index(absolute position, column A is 0, B is 1, ...). |
| [setOrder1()](#setorder1) | Represents sort order of the first key. The value of the property is SortOrder integer constant. |
| [setOrder2()](#setorder2) | Represents sort order of the second key. The value of the property is SortOrder integer constant. |
| [setOrder3()](#setorder3) | Represents sort order of the third key. The value of the property is SortOrder integer constant. |
| [setSortAsNumber()](#setsortasnumber) | Indicates whether sorting anything that looks like a number. |
| [setSortLeftToRight()](#setsortlefttoright) | True means that sorting orientation is from left to right. False means that sorting orientation is from top to bottom. T |
| [sort(cells, startRow, startColumn, endRow, endColumn)](#sort) | Sorts the data of the area. |
| [sort(cells, area)](#sort-1) | Sort the data of the area. |
| [sort()](#sort-2) | Sort the data in the range. |

### addColorKey() {#addcolorkey}

### addKey(key, order) {#addkey}

Adds sorted column index and sort order.

| Parameter | Type | Description |
| --- | --- | --- |
| key | Number | The sorted column index(absolute position, column A is 0, B is 1, ...) |
| order | Number | SortOrder |

### addKey(key, order, customList) {#addkey-1}

Adds sorted column index and sort order with custom sort list.

| Parameter | Type | Description |
| --- | --- | --- |
| key | Number | The sorted column index(absolute position, column A is 0, B is 1, ...) |
| order | Number | SortOrder |
| customList | String | The custom sort list. |

### addKey(key, type, order, customList) {#addkey-2}

Adds sorted column index and sort order with custom sort list. If type is SortOnType.CellColor or SortOnType.FontColor, the customList is Color.

| Parameter | Type | Description |
| --- | --- | --- |
| key | Number | The sorted column index(absolute position, column A is 0, B is 1, ...) |
| type | Number | SortOnType |
| order | Number | SortOrder |
| customList | Object | The custom sort list. |

### addKey(key, order, customList) {#addkey-3}

Adds sorted column index and sort order with custom sort list.

| Parameter | Type | Description |
| --- | --- | --- |
| key | Number | The sorted column index(absolute position, column A is 0, B is 1, ...) |
| order | Number | SortOrder |
| customList | Array of String | The custom sort list. |

### clear() {#clear}

Clear all settings.

### getCaseSensitive() {#getcasesensitive}

Gets and sets whether case sensitive when comparing string.

### getKey1() {#getkey1}

Represents first sorted column index(absolute position, column A is 0, B is 1, ...).

### getKey2() {#getkey2}

Represents second sorted column index(absolute position, column A is 0, B is 1, ...).

### getKey3() {#getkey3}

Represents third sorted column index(absolute position, column A is 0, B is 1, ...).

### getKeys() {#getkeys}

Gets the key list of data sorter.

### getOrder1() {#getorder1}

Represents sort order of the first key. The value of the property is SortOrder integer constant.

### getOrder2() {#getorder2}

Represents sort order of the second key. The value of the property is SortOrder integer constant.

### getOrder3() {#getorder3}

Represents sort order of the third key. The value of the property is SortOrder integer constant.

### getSortAsNumber() {#getsortasnumber}

Indicates whether sorting anything that looks like a number.

### getSortLeftToRight() {#getsortlefttoright}

True means that sorting orientation is from left to right. False means that sorting orientation is from top to bottom. The default value is false.

### hasHeaders() {#hasheaders}

Represents whether the range has headers.

### setCaseSensitive() {#setcasesensitive}

Gets and sets whether case sensitive when comparing string.

### setHasHeaders() {#sethasheaders}

Represents whether the range has headers.

### setKey1() {#setkey1}

Represents first sorted column index(absolute position, column A is 0, B is 1, ...).

### setKey2() {#setkey2}

Represents second sorted column index(absolute position, column A is 0, B is 1, ...).

### setKey3() {#setkey3}

Represents third sorted column index(absolute position, column A is 0, B is 1, ...).

### setOrder1() {#setorder1}

Represents sort order of the first key. The value of the property is SortOrder integer constant.

### setOrder2() {#setorder2}

Represents sort order of the second key. The value of the property is SortOrder integer constant.

### setOrder3() {#setorder3}

Represents sort order of the third key. The value of the property is SortOrder integer constant.

### setSortAsNumber() {#setsortasnumber}

Indicates whether sorting anything that looks like a number.

### setSortLeftToRight() {#setsortlefttoright}

True means that sorting orientation is from left to right. False means that sorting orientation is from top to bottom. The default value is false.

### sort(cells, startRow, startColumn, endRow, endColumn) {#sort}

Sorts the data of the area.

| Parameter | Type | Description |
| --- | --- | --- |
| cells | Cells | The cells contains the data area. |
| startRow | Number | The start row of the area. |
| startColumn | Number | The start column of the area. |
| endRow | Number | The end row of the area. |
| endColumn | Number | The end column of the area. |

**Returns:** Array of Number — `Array of Number` the original indices(absolute position, for example, column A is 0, B is 1, ...) of the sorted rows/columns. If no rows/columns needs to be moved by this sorting operation, null will be returned.

### sort(cells, area) {#sort-1}

Sort the data of the area.

| Parameter | Type | Description |
| --- | --- | --- |
| cells | Cells | The cells contains the data area. |
| area | CellArea | The area needed to sort |

**Returns:** Array of Number — `Array of Number` the original indices(absolute position, for example, column A is 0, B is 1, ...) of the sorted rows/columns. If no rows/columns needs to be moved by this sorting operation, null will be returned.

### sort() {#sort-2}

Sort the data in the range.

**Returns:** Array of Number — `Array of Number` the original indices(absolute position, for example, column A is 0, B is 1, ...) of the sorted rows/columns. If no rows/columns needs to be moved by this sorting operation, null will be returned.
