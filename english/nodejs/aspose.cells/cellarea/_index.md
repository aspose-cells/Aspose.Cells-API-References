---
title: "CellArea"
linktitle: "CellArea"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Represent an area of cells."
type: docs
weight: 350
url: /nodejs/aspose.cells/cellarea/
---

## CellArea class

Represent an area of cells.

```js
new CellArea()
```

## Properties

| Name | Description |
| --- | --- |
| [EndColumn](#endcolumn) | Gets or set the end column of this area. |
| [EndRow](#endrow) | Gets or set the end row of this area. |
| [StartColumn](#startcolumn) | Gets or set the start column of this area. |
| [StartRow](#startrow) | Gets or set the start row of this area. |

## Methods

| Name | Description |
| --- | --- |
| [compareTo(obj)](#compareto) | Compare two CellArea objects according to their top-left corner. |
| [toString()](#tostring) | Returns a string represents the current cell area object. |
| [createCellArea(startRow, startColumn, endRow, endColumn)](#createcellarea) *(static)* | Creates a cell area. |
| [createCellArea(startCellName, endCellName)](#createcellarea-1) *(static)* | Creates a cell area. |

### EndColumn {#endcolumn}

Gets or set the end column of this area.

### EndRow {#endrow}

Gets or set the end row of this area.

### StartColumn {#startcolumn}

Gets or set the start column of this area.

### StartRow {#startrow}

Gets or set the start row of this area.

### compareTo(obj) {#compareto}

Compare two CellArea objects according to their top-left corner.

| Parameter | Type | Description |
| --- | --- | --- |
| obj | Object |  |

**Returns:** Number — `Number` If two corners are in different rows, then compare their row index. Otherwise compare their column index. If two corners are same, then 0 will be returned.

### toString() {#tostring}

Returns a string represents the current cell area object.

**Returns:** String — `String`

### createCellArea(startRow, startColumn, endRow, endColumn) (static) {#createcellarea}

Creates a cell area.

| Parameter | Type | Description |
| --- | --- | --- |
| startRow | Number | The start row. |
| startColumn | Number | The start column. |
| endRow | Number | The end row. |
| endColumn | Number | The end column. |

**Returns:** CellArea — `CellArea` Return a CellArea.

### createCellArea(startCellName, endCellName) (static) {#createcellarea-1}

Creates a cell area.

| Parameter | Type | Description |
| --- | --- | --- |
| startCellName | String | The top-left cell of the range. |
| endCellName | String | The bottom-right cell of the range. |

**Returns:** CellArea — `CellArea` Return a CellArea.
