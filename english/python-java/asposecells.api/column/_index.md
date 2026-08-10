---
title: "Column Class"
linktitle: "Column"
articleTitle: "Column"
second_title: "Aspose.Cells for Python via Java"
description: "Represents a single column in a worksheet."
type: docs
weight: 1000
url: /python-java/asposecells.api/column/
---

## Column class

Represents a single column in a worksheet.

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [Index](#index) | int | Gets the index of this column. |
| [Width](#width) | float | Gets and sets the column width in unit of characters. For spreadsheet, column width is measured as the number of charact |
| [GroupLevel](#grouplevel) | byte | Gets the group level of the column. |
| [IsHidden](#ishidden) | boolean | Indicates whether the column is hidden. |
| [HasCustomStyle](#hascustomstyle) | boolean | Indicates whether this column has custom style settings(different from the default one inherited from workbook). |
| [IsCollapsed](#iscollapsed) | boolean | whether the column is collapsed |

## Methods

| Name | Description |
| --- | --- |
| [applyStyle](#applystyle) | Applies formats for a whole column. |
| [getStyle](#getstyle) | Gets the style of this column.

Modifying the returned style object directly takes no effect for this column or any cell |
| [setStyle](#setstyle) | Sets the style of this column.

This method only sets the given style as the default style for this column, without chan |

### Column.Index property {#index}

Gets the index of this column.

**Type:** int

### Column.Width property {#width}

Gets and sets the column width in unit of characters. For spreadsheet, column width is measured as the number of characters of the maximum digit width of the numbers 0~9 as rendered in the normal style's font.

**Type:** float

### Column.GroupLevel property {#grouplevel}

Gets the group level of the column.

**Type:** byte

### Column.IsHidden property {#ishidden}

Indicates whether the column is hidden.

**Type:** boolean

### Column.HasCustomStyle property {#hascustomstyle}

Indicates whether this column has custom style settings(different from the default one inherited from workbook).

**Type:** boolean

### Column.IsCollapsed property {#iscollapsed}

whether the column is collapsed

**Type:** boolean

### applyStyle(style, flag) {#applystyle}

Applies formats for a whole column.

| Parameter | Type | Description |
| --- | --- | --- |
| style | Style | The style object which will be applied. |
| flag | StyleFlag | Flags which indicates applied formatting properties. |

### getStyle() {#getstyle}

Gets the style of this column.

Modifying the returned style object directly takes no effect for this column or any cells in this column. You have to call applyStyle(com.aspose.cells.Style, com.aspose.cells.StyleFlag) or setStyle(com.aspose.cells.Style) method to apply the change to this column. Column's style is the style which will be inherited by cells in this column(those cells that have no custom style settings, such as existing cells that have not been set style explicitly, or those that have not been instantiated)

### setStyle(style) {#setstyle}

Sets the style of this column.

This method only sets the given style as the default style for this column, without changing the style settings for existing cells in this column. To update style settings of existing cells to the specified style at the same time, please use applyStyle(com.aspose.cells.Style, com.aspose.cells.StyleFlag)

| Parameter | Type | Description |
| --- | --- | --- |
| style | Style | the style to be used as the default style for cells in this column. |
