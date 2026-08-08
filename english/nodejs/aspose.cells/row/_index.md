---
title: "Row"
linktitle: "Row"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Represents a single row in a worksheet."
type: docs
weight: 3390
url: /nodejs/aspose.cells/row/
---

## Row class

Represents a single row in a worksheet.

## Methods

| Name | Description |
| --- | --- |
| [applyStyle(style, flag)](#applystyle) | Applies formats for a whole row. |
| [copySettings(source, checkStyle)](#copysettings) | Copy settings of row, such as style, height, visibility, ...etc. |
| [equals(obj)](#equals) | Checks whether this object refers to the same row with another. |
| [equals(row)](#equals-1) | Checks whether this object refers to the same row with another row object. |
| [get(column)](#get) | Gets the cell. |
| [getCellByIndex(index)](#getcellbyindex) | Get the cell by specific index in the cells collection of this row. To traverse all cells in sequence without modificati |
| [getCellOrNull(column)](#getcellornull) | Gets the cell or null in the specific index. |
| [getFirstCell()](#getfirstcell) | Gets the first cell object in the row. |
| [getFirstDataCell()](#getfirstdatacell) | Gets the first non-blank cell in the row. |
| [getGroupLevel()](#getgrouplevel) | Gets the group level of the row. |
| [getHeight()](#getheight) | Gets and sets the row height in unit of Points. |
| [getIndex()](#getindex) | Gets the index of this row. |
| [getLastCell()](#getlastcell) | Gets the last cell object in the row. |
| [getLastDataCell()](#getlastdatacell) | Gets the last non-blank cell in the row. |
| [getStyle()](#getstyle) | Gets the style of this row. Modifying the returned style object directly takes no effect for this row or any cells in th |
| [hasCustomStyle()](#hascustomstyle) | Indicates whether this row has custom style settings(different from the default one inherited from workbook). |
| [isBlank()](#isblank) | Indicates whether the row contains any data |
| [isCollapsed()](#iscollapsed) | whether the row is collapsed |
| [isHeightMatched()](#isheightmatched) | Indicates whether the row height matches current default font setting of the workbook. True of this property also denote |
| [isHidden()](#ishidden) | Indicates whether the row is hidden. |
| [iterator()](#iterator) | Gets the cells enumerator |
| [setCollapsed()](#setcollapsed) | whether the row is collapsed |
| [setGroupLevel()](#setgrouplevel) | Gets the group level of the row. |
| [setHeight()](#setheight) | Gets and sets the row height in unit of Points. |
| [setHeightMatched()](#setheightmatched) | Indicates whether the row height matches current default font setting of the workbook. True of this property also denote |
| [setHidden()](#sethidden) | Indicates whether the row is hidden. |
| [setStyle(style)](#setstyle) | Sets the style of this row. This method only sets the given style as the default style for this row, without changing th |

### applyStyle(style, flag) {#applystyle}

Applies formats for a whole row.

| Parameter | Type | Description |
| --- | --- | --- |
| style | Style | The style object which will be applied. |
| flag | StyleFlag | Flags which indicates applied formatting properties. |

### copySettings(source, checkStyle) {#copysettings}

Copy settings of row, such as style, height, visibility, ...etc.

| Parameter | Type | Description |
| --- | --- | --- |
| source | Row | the source row whose settings will be copied to this one |
| checkStyle | boolean | whether check and gather style. Only takes effect and be needed when two row objects belong to different workbook and the styles of two workbooks are different. |

### equals(obj) {#equals}

Checks whether this object refers to the same row with another.

| Parameter | Type | Description |
| --- | --- | --- |
| obj | Object | another object |

**Returns:** boolean — `boolean` true if two objects refers to the same row.

### equals(row) {#equals-1}

Checks whether this object refers to the same row with another row object.

| Parameter | Type | Description |
| --- | --- | --- |
| row | Row | another row object |

**Returns:** boolean — `boolean` true if two row objects refers to the same row.

### get(column) {#get}

Gets the cell.

| Parameter | Type | Description |
| --- | --- | --- |
| column | Number | The column index |

**Returns:** Cell — `Cell`

### getCellByIndex(index) {#getcellbyindex}

Get the cell by specific index in the cells collection of this row. To traverse all cells in sequence without modification, using iterator() will give better performance than using this method to get cell one by one.

| Parameter | Type | Description |
| --- | --- | --- |
| index | Number | The index(position) of the cell in the cells collection of this row. |

**Returns:** Cell — `Cell` The Cell object at given position.

### getCellOrNull(column) {#getcellornull}

Gets the cell or null in the specific index.

| Parameter | Type | Description |
| --- | --- | --- |
| column | Number | The column index |

**Returns:** Cell — `Cell` Returns the cell object if the cell exists. Or returns null if the cell object does not exist.

### getFirstCell() {#getfirstcell}

Gets the first cell object in the row.

### getFirstDataCell() {#getfirstdatacell}

Gets the first non-blank cell in the row.

### getGroupLevel() {#getgrouplevel}

Gets the group level of the row.

### getHeight() {#getheight}

Gets and sets the row height in unit of Points.

### getIndex() {#getindex}

Gets the index of this row.

### getLastCell() {#getlastcell}

Gets the last cell object in the row.

### getLastDataCell() {#getlastdatacell}

Gets the last non-blank cell in the row.

### getStyle() {#getstyle}

Gets the style of this row. Modifying the returned style object directly takes no effect for this row or any cells in this row. You have to call applyStyle(com.aspose.cells.Style, com.aspose.cells.StyleFlag) or setStyle(com.aspose.cells.Style) method to apply the change to this row. Row's style is the style which will be inherited by cells in this row(those cells that have no custom style settings, such as existing cells that have not been set style explicitly, or those that have not been instantiated)

### hasCustomStyle() {#hascustomstyle}

Indicates whether this row has custom style settings(different from the default one inherited from workbook).

### isBlank() {#isblank}

Indicates whether the row contains any data

### isCollapsed() {#iscollapsed}

whether the row is collapsed

### isHeightMatched() {#isheightmatched}

Indicates whether the row height matches current default font setting of the workbook. True of this property also denotes the row height is "automatic" without custom height value set by user. When this property is true, if the content in this row changes, generally the row height needs to be re-calculated(such as by Worksheet.autoFitRows()) to get the same result with what is shown in ms excel when you opening the workbook in it.

### isHidden() {#ishidden}

Indicates whether the row is hidden.

### iterator() {#iterator}

Gets the cells enumerator

**Returns:** Iterator — `Iterator` The cells enumerator

### setCollapsed() {#setcollapsed}

whether the row is collapsed

### setGroupLevel() {#setgrouplevel}

Gets the group level of the row.

### setHeight() {#setheight}

Gets and sets the row height in unit of Points.

### setHeightMatched() {#setheightmatched}

Indicates whether the row height matches current default font setting of the workbook. True of this property also denotes the row height is "automatic" without custom height value set by user. When this property is true, if the content in this row changes, generally the row height needs to be re-calculated(such as by Worksheet.autoFitRows()) to get the same result with what is shown in ms excel when you opening the workbook in it.

### setHidden() {#sethidden}

Indicates whether the row is hidden.

### setStyle(style) {#setstyle}

Sets the style of this row. This method only sets the given style as the default style for this row, without changing the style settings for existing cells in this row. To update style settings of existing cells to the specified style at the same time, please use applyStyle(com.aspose.cells.Style, com.aspose.cells.StyleFlag)

| Parameter | Type | Description |
| --- | --- | --- |
| style | Style | the style to be used as the default style for cells in this row. |
