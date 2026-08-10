---
title: "Row Class"
linktitle: "Row"
articleTitle: "Row"
second_title: "Aspose.Cells for PHP via Java"
description: "Represents a single row in a worksheet."
type: docs
weight: 5610
url: /php/aspose.cells/row/
---

## Row class

Represents a single row in a worksheet.

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [IsBlank](#isblank) | boolean | Indicates whether the row contains any data |
| [IsCollapsed](#iscollapsed) | boolean | whether the row is collapsed |
| [Height](#height) | Number | Gets and sets the row height in unit of Points. |
| [IsHidden](#ishidden) | boolean | Indicates whether the row is hidden. |
| [Index](#index) | Number | Gets the index of this row. |
| [GroupLevel](#grouplevel) | byte | Gets the group level of the row. |
| [IsHeightMatched](#isheightmatched) | boolean | Indicates whether the row height matches current default font setting of the workbook. True of this property also denote |
| [HasCustomStyle](#hascustomstyle) | boolean | Indicates whether this row has custom style settings(different from the default one inherited from workbook). |
| [FirstCell](#firstcell) | Cell | Gets the first cell object in the row. |
| [FirstDataCell](#firstdatacell) | Cell | Gets the first non-blank cell in the row. |
| [LastCell](#lastcell) | Cell | Gets the last cell object in the row. |
| [LastDataCell](#lastdatacell) | Cell | Gets the last non-blank cell in the row. |
| [Item (int)](#itemint) | Cell | Gets the cell. |

## Methods

| Name | Description |
| --- | --- |
| [getCellByIndex](#getcellbyindex) | Get the cell by specific index in the cells collection of this row.

To traverse all cells in sequence without modificat |
| [iterator](#iterator) | Gets the cells enumerator |
| [getCellOrNull](#getcellornull) | Gets the cell or null in the specific index. |
| [getStyle](#getstyle) | Gets the style of this row.

Modifying the returned style object directly takes no effect for this row or any cells in t |
| [setStyle](#setstyle) | Sets the style of this row.

This method only sets the given style as the default style for this row, without changing t |
| [copySettings](#copysettings) | Copy settings of row, such as style, height, visibility, ...etc. |
| [applyStyle](#applystyle) | Applies formats for a whole row. |
| [equals](#equals) | Checks whether this object refers to the same row with another. |

### Row.IsBlank property {#isblank}

Indicates whether the row contains any data

**Type:** boolean

### Row.IsCollapsed property {#iscollapsed}

whether the row is collapsed

**Type:** boolean

### Row.Height property {#height}

Gets and sets the row height in unit of Points.

**Type:** Number

### Row.IsHidden property {#ishidden}

Indicates whether the row is hidden.

**Type:** boolean

### Row.Index property {#index}

Gets the index of this row.

**Type:** Number

### Row.GroupLevel property {#grouplevel}

Gets the group level of the row.

**Type:** byte

### Row.IsHeightMatched property {#isheightmatched}

Indicates whether the row height matches current default font setting of the workbook. True of this property also denotes the row height is "automatic" without custom height value set by user. When this property is true, if the content in this row changes, generally the row height needs to be re-calculated(such as by Worksheet.autoFitRows() ) to get the same result with what is shown in ms excel when you opening the workbook in it.

**Type:** boolean

### Row.HasCustomStyle property {#hascustomstyle}

Indicates whether this row has custom style settings(different from the default one inherited from workbook).

**Type:** boolean

### Row.FirstCell property {#firstcell}

Gets the first cell object in the row.

**Type:** Cell

### Row.FirstDataCell property {#firstdatacell}

Gets the first non-blank cell in the row.

**Type:** Cell

### Row.LastCell property {#lastcell}

Gets the last cell object in the row.

**Type:** Cell

### Row.LastDataCell property {#lastdatacell}

Gets the last non-blank cell in the row.

**Type:** Cell

### Row.Item (int) property {#itemint}

Gets the cell.

**Type:** Cell

### getCellByIndex(index) {#getcellbyindex}

Get the cell by specific index in the cells collection of this row.

To traverse all cells in sequence without modification, using iterator() will give better performance than using this method to get cell one by one.

| Parameter | Type | Description |
| --- | --- | --- |
| index | Number | The index(position) of the cell in the cells collection of this row. |

**Returns:** The Cell object at given position.

### iterator() {#iterator}

Gets the cells enumerator

**Returns:** The cells enumerator

### getCellOrNull(column) {#getcellornull}

Gets the cell or null in the specific index.

| Parameter | Type | Description |
| --- | --- | --- |
| column | Number | The column index |

**Returns:** Returns the cell object if the cell exists. Or returns null if the cell object does not exist.

### getStyle() {#getstyle}

Gets the style of this row.

Modifying the returned style object directly takes no effect for this row or any cells in this row. You have to call applyStyle(com.aspose.cells.Style, com.aspose.cells.StyleFlag) or setStyle(com.aspose.cells.Style) method to apply the change to this row. Row's style is the style which will be inherited by cells in this row(those cells that have no custom style settings, such as existing cells that have not been set style explicitly, or those that have not been instantiated)

### setStyle(style) {#setstyle}

Sets the style of this row.

This method only sets the given style as the default style for this row, without changing the style settings for existing cells in this row. To update style settings of existing cells to the specified style at the same time, please use applyStyle(com.aspose.cells.Style, com.aspose.cells.StyleFlag)

| Parameter | Type | Description |
| --- | --- | --- |
| style | Style | the style to be used as the default style for cells in this row. |

### copySettings(source, checkStyle) {#copysettings}

Copy settings of row, such as style, height, visibility, ...etc.

| Parameter | Type | Description |
| --- | --- | --- |
| source | Row | the source row whose settings will be copied to this one |
| checkStyle | boolean | whether check and gather style. Only takes effect and be needed when two row objects belong to different workbook and the styles of two workbooks are different. |

### applyStyle(style, flag) {#applystyle}

Applies formats for a whole row.

| Parameter | Type | Description |
| --- | --- | --- |
| style | Style | The style object which will be applied. |
| flag | StyleFlag | Flags which indicates applied formatting properties. |

### equals(obj) (1 of 2) {#equals}

Checks whether this object refers to the same row with another.

| Parameter | Type | Description |
| --- | --- | --- |
| obj | Object | another object |

**Returns:** true if two objects refers to the same row.

---

### equals(row) (2 of 2) {#equals-1}

Checks whether this object refers to the same row with another row object.

| Parameter | Type | Description |
| --- | --- | --- |
| row | Row | another row object |

**Returns:** true if two row objects refers to the same row.
