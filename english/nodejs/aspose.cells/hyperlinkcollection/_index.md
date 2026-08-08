---
title: "HyperlinkCollection"
linktitle: "HyperlinkCollection"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Encapsulates a collection of Hyperlink objects."
type: docs
weight: 1850
url: /nodejs/aspose.cells/hyperlinkcollection/
---

## HyperlinkCollection class

Encapsulates a collection of Hyperlink objects.

## Methods

| Name | Description |
| --- | --- |
| [add(firstRow, firstColumn, totalRows, totalColumns, address)](#add) | Adds a hyperlink to a specified cell or a range of cells. |
| [add(cellName, totalRows, totalColumns, address)](#add-1) | Adds a hyperlink to a specified cell or a range of cells. |
| [add(startCellName, endCellName, address, textToDisplay, screenTip)](#add-2) | Adds a hyperlink to a specified cell or a range of cells. |
| [add()](#add-3) | Reserved for internal use. |
| [clear()](#clear) | Clears all hyperlinks. |
| [contains()](#contains) | Reserved for internal use. |
| [get(index)](#get) | Gets the Hyperlink element at the specified index. |
| [get()](#get-1) | Reserved for internal use. |
| [getCount()](#getcount) |  |
| [indexOf()](#indexof) | Reserved for internal use. |
| [iterator()](#iterator) |  |
| [removeAt(index)](#removeat) | Remove the hyperlink at the specified index in this collection. |

### add(firstRow, firstColumn, totalRows, totalColumns, address) {#add}

Adds a hyperlink to a specified cell or a range of cells.

| Parameter | Type | Description |
| --- | --- | --- |
| firstRow | Number | First row of the hyperlink range. |
| firstColumn | Number | First column of the hyperlink range. |
| totalRows | Number | Number of rows in this hyperlink range. |
| totalColumns | Number | Number of columns of this hyperlink range. |
| address | String | Address of the hyperlink. |

**Returns:** Number — `Number` Hyperlink object index.

**Example:**

```js
var excel = new aspose.cells.Workbook();
var worksheet = excel.getWorksheets().get(0);
worksheet.getHyperlinks().add("A4", 1, 1, "http://www.aspose.com");
worksheet.getHyperlinks().add("A5", 1, 1, "c:\\book1.xls");
```

### add(cellName, totalRows, totalColumns, address) {#add-1}

Adds a hyperlink to a specified cell or a range of cells.

| Parameter | Type | Description |
| --- | --- | --- |
| cellName | String | Cell name. |
| totalRows | Number | Number of rows in this hyperlink range. |
| totalColumns | Number | Number of columns of this hyperlink range. |
| address | String | Address of the hyperlink. |

**Returns:** Number — `Number` Hyperlink object index.

### add(startCellName, endCellName, address, textToDisplay, screenTip) {#add-2}

Adds a hyperlink to a specified cell or a range of cells.

| Parameter | Type | Description |
| --- | --- | --- |
| startCellName | String | The top-left cell of the range. |
| endCellName | String | The bottom-right cell of the range. |
| address | String | Address of the hyperlink. |
| textToDisplay | String | The text to be displayed for the specified hyperlink. |
| screenTip | String | The screenTip text for the specified hyperlink. |

**Returns:** Number — `Number` Hyperlink object index.

### add() {#add-3}

Reserved for internal use.

### clear() {#clear}

Clears all hyperlinks.

### contains() {#contains}

Reserved for internal use.

### get(index) {#get}

Gets the Hyperlink element at the specified index.

| Parameter | Type | Description |
| --- | --- | --- |
| index | Number | The zero based index of the element. |

**Returns:** Hyperlink — `Hyperlink` The element at the specified index.

### get() {#get-1}

Reserved for internal use.

### getCount() {#getcount}

### indexOf() {#indexof}

Reserved for internal use.

### iterator() {#iterator}

### removeAt(index) {#removeat}

Remove the hyperlink at the specified index in this collection.

| Parameter | Type | Description |
| --- | --- | --- |
| index | Number | The zero based index of the element. |
