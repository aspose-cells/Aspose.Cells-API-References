---
title: "HyperlinkCollection Class"
linktitle: "HyperlinkCollection"
articleTitle: "HyperlinkCollection"
second_title: "Aspose.Cells for PHP via Java"
description: "Encapsulates a collection of Hyperlink objects."
type: docs
weight: 3020
url: /php/aspose.cells/hyperlinkcollection/
---

## HyperlinkCollection class

Encapsulates a collection of Hyperlink objects.

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [Count](#count) | Number |  |
| [Item (int)](#itemint) | Hyperlink | Gets the Hyperlink element at the specified index. |

## Methods

| Name | Description |
| --- | --- |
| [add](#add) | Adds a hyperlink to a specified cell or a range of cells. |
| [removeAt](#removeat) | Remove the hyperlink at the specified index in this collection. |
| [clear](#clear) | Clears all hyperlinks. |
| [iterator](#iterator) |  |
| [get](#get) | Reserved for internal use. |
| [contains](#contains) | Reserved for internal use. |
| [indexOf](#indexof) | Reserved for internal use. |

### HyperlinkCollection.Count property {#count}

**Type:** Number

### HyperlinkCollection.Item (int) property {#itemint}

Gets the Hyperlink element at the specified index.

**Type:** Hyperlink

### add(firstRow, firstColumn, totalRows, totalColumns, address) (1 of 4) {#add}

Adds a hyperlink to a specified cell or a range of cells.

| Parameter | Type | Description |
| --- | --- | --- |
| firstRow | Number | First row of the hyperlink range. |
| firstColumn | Number | First column of the hyperlink range. |
| totalRows | Number | Number of rows in this hyperlink range. |
| totalColumns | Number | Number of columns of this hyperlink range. |
| address | String | Address of the hyperlink. |

**Returns:** Hyperlink object index.

**Example:**

```php
$workbook = new cells\Workbook();
$worksheet = $workbook->getWorksheets()->get(0);
$worksheet->getHyperlinks()->add("A4", 1, 1, "http://www.aspose.com");
$worksheet->getHyperlinks()->add("A5", 1, 1, "c:\\book1.xls");
```

---

### add(cellName, totalRows, totalColumns, address) (2 of 4) {#add-1}

Adds a hyperlink to a specified cell or a range of cells.

| Parameter | Type | Description |
| --- | --- | --- |
| cellName | String | Cell name. |
| totalRows | Number | Number of rows in this hyperlink range. |
| totalColumns | Number | Number of columns of this hyperlink range. |
| address | String | Address of the hyperlink. |

**Returns:** Hyperlink object index.

---

### add(startCellName, endCellName, address, textToDisplay, screenTip) (3 of 4) {#add-2}

Adds a hyperlink to a specified cell or a range of cells.

| Parameter | Type | Description |
| --- | --- | --- |
| startCellName | String | The top-left cell of the range. |
| endCellName | String | The bottom-right cell of the range. |
| address | String | Address of the hyperlink. |
| textToDisplay | String | The text to be displayed for the specified hyperlink. |
| screenTip | String | The screenTip text for the specified hyperlink. |

**Returns:** Hyperlink object index.

---

### add(value) (4 of 4) {#add-3}

Reserved for internal use.

### removeAt(index) {#removeat}

Remove the hyperlink at the specified index in this collection.

| Parameter | Type | Description |
| --- | --- | --- |
| index | Number | The zero based index of the element. |

### clear() {#clear}

Clears all hyperlinks.

### iterator() {#iterator}

### get(index) {#get}

Reserved for internal use.

### contains(value) {#contains}

Reserved for internal use.

### indexOf(value) {#indexof}

Reserved for internal use.
