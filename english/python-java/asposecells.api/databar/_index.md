---
title: "DataBar Class"
linktitle: "DataBar"
articleTitle: "DataBar"
second_title: "Aspose.Cells for Python via Java"
description: "Describe the DataBar conditional formatting rule."
type: docs
weight: 1490
url: /python-java/asposecells.api/databar/
---

## DataBar class

Describe the DataBar conditional formatting rule. This conditional formatting rule displays a gradated data bar in the range of cells.

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [AxisColor](#axiscolor) | Color | Gets the color of the axis for cells with conditional formatting as data bars. |
| [AxisPosition](#axisposition) | int | Gets or sets the position of the axis of the data bars specified by a conditional formatting rule. The value of the prop |
| [BarFillType](#barfilltype) | int | Gets or sets how a data bar is filled with color. The value of the property is DataBarFillType integer constant. |
| [Direction](#direction) | int | Gets or sets the direction the databar is displayed. The value of the property is TextDirectionType integer constant. |
| [BarBorder](#barborder) | DataBarBorder | Gets an object that specifies the border of a data bar. |
| [NegativeBarFormat](#negativebarformat) | NegativeBarFormat | Gets the NegativeBarFormat object associated with a data bar conditional formatting rule. |
| [MinCfvo](#mincfvo) | ConditionalFormattingValue | Get or set this DataBar's min value object. Cannot set null or CFValueObject with type FormatConditionValueType.Max to i |
| [MaxCfvo](#maxcfvo) | ConditionalFormattingValue | Get or set this DataBar's max value object. Cannot set null or CFValueObject with type FormatConditionValueType.Min to i |
| [Color](#color) | Color | Get or set this DataBar's Color. |
| [MinLength](#minlength) | int | Represents the min length of data bar . |
| [MaxLength](#maxlength) | int | Represents the max length of data bar . |
| [ShowValue](#showvalue) | boolean | Get or set the flag indicating whether to show the values of the cells on which this data bar is applied. Default value  |

## Methods

| Name | Description |
| --- | --- |
| [toImage](#toimage) | Render data bar in cell to image byte array. |

### DataBar.AxisColor property {#axiscolor}

Gets the color of the axis for cells with conditional formatting as data bars.

**Type:** Color

### DataBar.AxisPosition property {#axisposition}

Gets or sets the position of the axis of the data bars specified by a conditional formatting rule. The value of the property is DataBarAxisPosition integer constant.

**Type:** int

### DataBar.BarFillType property {#barfilltype}

Gets or sets how a data bar is filled with color. The value of the property is DataBarFillType integer constant.

**Type:** int

### DataBar.Direction property {#direction}

Gets or sets the direction the databar is displayed. The value of the property is TextDirectionType integer constant.

**Type:** int

### DataBar.BarBorder property {#barborder}

Gets an object that specifies the border of a data bar.

**Type:** DataBarBorder

### DataBar.NegativeBarFormat property {#negativebarformat}

Gets the NegativeBarFormat object associated with a data bar conditional formatting rule.

**Type:** NegativeBarFormat

### DataBar.MinCfvo property {#mincfvo}

Get or set this DataBar's min value object. Cannot set null or CFValueObject with type FormatConditionValueType.Max to it.

**Type:** ConditionalFormattingValue

### DataBar.MaxCfvo property {#maxcfvo}

Get or set this DataBar's max value object. Cannot set null or CFValueObject with type FormatConditionValueType.Min to it.

**Type:** ConditionalFormattingValue

### DataBar.Color property {#color}

Get or set this DataBar's Color.

**Type:** Color

### DataBar.MinLength property {#minlength}

Represents the min length of data bar .

**Type:** int

### DataBar.MaxLength property {#maxlength}

Represents the max length of data bar .

**Type:** int

### DataBar.ShowValue property {#showvalue}

Get or set the flag indicating whether to show the values of the cells on which this data bar is applied. Default value is true.

**Type:** boolean

### toImage(cell, imgOpts) {#toimage}

Render data bar in cell to image byte array.

| Parameter | Type | Description |
| --- | --- | --- |
| cell | Cell | Indicate the data bar in which cell to be rendered |
| imgOpts | ImageOrPrintOptions | ImageOrPrintOptions contains some property of output image |
