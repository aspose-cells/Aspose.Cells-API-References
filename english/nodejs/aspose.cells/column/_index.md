---
title: "Column"
linktitle: "Column"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Represents a single column in a worksheet."
type: docs
weight: 680
url: /nodejs/aspose.cells/column/
---

## Column class

Represents a single column in a worksheet.

## Methods

| Name | Description |
| --- | --- |
| [applyStyle(style, flag)](#applystyle) | Applies formats for a whole column. |
| [getGroupLevel()](#getgrouplevel) | Gets the group level of the column. |
| [getIndex()](#getindex) | Gets the index of this column. |
| [getStyle()](#getstyle) | Gets the style of this column. Modifying the returned style object directly takes no effect for this column or any cells |
| [getWidth()](#getwidth) | Gets and sets the column width in unit of characters. For spreadsheet, column width is measured as the number of charact |
| [hasCustomStyle()](#hascustomstyle) | Indicates whether this column has custom style settings(different from the default one inherited from workbook). |
| [isCollapsed()](#iscollapsed) | whether the column is collapsed |
| [isHidden()](#ishidden) | Indicates whether the column is hidden. |
| [setCollapsed()](#setcollapsed) | whether the column is collapsed |
| [setGroupLevel()](#setgrouplevel) | Gets the group level of the column. |
| [setHidden()](#sethidden) | Indicates whether the column is hidden. |
| [setStyle(style)](#setstyle) | Sets the style of this column. This method only sets the given style as the default style for this column, without chang |
| [setWidth()](#setwidth) | Gets and sets the column width in unit of characters. For spreadsheet, column width is measured as the number of charact |

### applyStyle(style, flag) {#applystyle}

Applies formats for a whole column.

| Parameter | Type | Description |
| --- | --- | --- |
| style | Style | The style object which will be applied. |
| flag | StyleFlag | Flags which indicates applied formatting properties. |

### getGroupLevel() {#getgrouplevel}

Gets the group level of the column.

### getIndex() {#getindex}

Gets the index of this column.

### getStyle() {#getstyle}

Gets the style of this column. Modifying the returned style object directly takes no effect for this column or any cells in this column. You have to call applyStyle(com.aspose.cells.Style, com.aspose.cells.StyleFlag) or setStyle(com.aspose.cells.Style) method to apply the change to this column. Column's style is the style which will be inherited by cells in this column(those cells that have no custom style settings, such as existing cells that have not been set style explicitly, or those that have not been instantiated)

### getWidth() {#getwidth}

Gets and sets the column width in unit of characters. For spreadsheet, column width is measured as the number of characters of the maximum digit width of the numbers 0~9 as rendered in the normal style's font.

### hasCustomStyle() {#hascustomstyle}

Indicates whether this column has custom style settings(different from the default one inherited from workbook).

### isCollapsed() {#iscollapsed}

whether the column is collapsed

### isHidden() {#ishidden}

Indicates whether the column is hidden.

### setCollapsed() {#setcollapsed}

whether the column is collapsed

### setGroupLevel() {#setgrouplevel}

Gets the group level of the column.

### setHidden() {#sethidden}

Indicates whether the column is hidden.

### setStyle(style) {#setstyle}

Sets the style of this column. This method only sets the given style as the default style for this column, without changing the style settings for existing cells in this column. To update style settings of existing cells to the specified style at the same time, please use applyStyle(com.aspose.cells.Style, com.aspose.cells.StyleFlag)

| Parameter | Type | Description |
| --- | --- | --- |
| style | Style | the style to be used as the default style for cells in this column. |

### setWidth() {#setwidth}

Gets and sets the column width in unit of characters. For spreadsheet, column width is measured as the number of characters of the maximum digit width of the numbers 0~9 as rendered in the normal style's font.
