---
title: DataBar
second_title: Aspose.Cells for JavaScript via C++ API Reference
description: Describe the DataBar conditional formatting rule. This conditional formatting rule displays a gradated data bar in the range of cells.
type: docs
url: /zh/javascript-cpp/databar/
---

## DataBar class

Describe the DataBar conditional formatting rule. This conditional formatting rule displays a gradated data bar in the range of cells.

```javascript
class DataBar;
```


### Example
```javascript
const { Workbook, CellArea, Color, FormatConditionType, FormatConditionValueType, SaveFormat } = AsposeCells;

//实例化一个 Workbook 对象
var workbook = new Workbook();
var sheet = workbook.worksheets.get(0);

//添加空的条件格式
var index = sheet.conditionalFormattings.add();
var fcs = sheet.conditionalFormattings.get(index);

//设置条件格式范围。
var ca = new CellArea();
ca.startRow = 0;
ca.endRow = 2;
ca.startColumn = 0;
ca.endColumn = 0;
fcs.addArea(ca);

//添加条件。
var idx = fcs.addCondition(FormatConditionType.DataBar);
fcs.addArea(ca);
var cond = fcs.get(idx);

//获取数据条
var dataBar = cond.dataBar;
var orange = Color.Orange;
dataBar.color = orange;

//设置数据条属性
dataBar.minCfvo.type = FormatConditionValueType.Percentile;
dataBar.minCfvo.value = 30;
dataBar.showValue = false;

//放置单元格值
var cell1 = sheet.cells.get("A1");
cell1.putValue(10);
var cell2 = sheet.cells.get("A2");
cell2.putValue(120);
var cell3 = sheet.cells.get("A3");
cell3.putValue(260);

//保存 Excel 文件
var uint8Array = workbook.save(SaveFormat.Xlsx);
```
## Properties

| Property | Type | Description |
| --- | --- | --- |
| [axisColor](#axisColor--)| Color | Gets the color of the axis for cells with conditional formatting as data bars. |
| [axisPosition](#axisPosition--)| DataBarAxisPosition | Gets or sets the position of the axis of the data bars specified by a conditional formatting rule. |
| [barFillType](#barFillType--)| DataBarFillType | Gets or sets how a data bar is filled with color. |
| [direction](#direction--)| TextDirectionType | Gets or sets the direction the databar is displayed. |
| [barBorder](#barBorder--)| DataBarBorder | Readonly. Gets an object that specifies the border of a data bar. |
| [negativeBarFormat](#negativeBarFormat--)| NegativeBarFormat | Readonly. Gets the NegativeBarFormat object associated with a data bar conditional formatting rule. |
| [minCfvo](#minCfvo--)| ConditionalFormattingValue | Readonly. Get or set this DataBar's min value object. Cannot set null or CFValueObject with type FormatConditionValueType.Max to it. |
| [maxCfvo](#maxCfvo--)| ConditionalFormattingValue | Readonly. Get or set this DataBar's max value object. Cannot set null or CFValueObject with type FormatConditionValueType.Min to it. |
| [color](#color--)| Color | Get or set this DataBar's Color. |
| [minLength](#minLength--)| number | Represents the min length of data bar . |
| [maxLength](#maxLength--)| number | Represents the max length of data bar . |
| [showValue](#showValue--)| boolean | Get or set the flag indicating whether to show the values of the cells on which this data bar is applied. Default value is true. |

## Methods

| Method | Description |
| --- | --- |
| [toImage(Cell, ImageOrPrintOptions)](#toImage-cell-imageorprintoptions-)| Render data bar in cell to image byte array. |


### axisColor {#axisColor--}

Gets the color of the axis for cells with conditional formatting as data bars.

```javascript
axisColor : Color;
```


### axisPosition {#axisPosition--}

Gets or sets the position of the axis of the data bars specified by a conditional formatting rule.

```javascript
axisPosition : DataBarAxisPosition;
```


### barFillType {#barFillType--}

Gets or sets how a data bar is filled with color.

```javascript
barFillType : DataBarFillType;
```


### direction {#direction--}

Gets or sets the direction the databar is displayed.

```javascript
direction : TextDirectionType;
```


### barBorder {#barBorder--}

Readonly. Gets an object that specifies the border of a data bar.

```javascript
barBorder : DataBarBorder;
```


### negativeBarFormat {#negativeBarFormat--}

Readonly. Gets the NegativeBarFormat object associated with a data bar conditional formatting rule.

```javascript
negativeBarFormat : NegativeBarFormat;
```


### minCfvo {#minCfvo--}

Readonly. Get or set this DataBar's min value object. Cannot set null or CFValueObject with type FormatConditionValueType.Max to it.

```javascript
minCfvo : ConditionalFormattingValue;
```


### maxCfvo {#maxCfvo--}

Readonly. Get or set this DataBar's max value object. Cannot set null or CFValueObject with type FormatConditionValueType.Min to it.

```javascript
maxCfvo : ConditionalFormattingValue;
```


### color {#color--}

Get or set this DataBar's Color.

```javascript
color : Color;
```


### minLength {#minLength--}

Represents the min length of data bar .

```javascript
minLength : number;
```


### maxLength {#maxLength--}

Represents the max length of data bar .

```javascript
maxLength : number;
```


### showValue {#showValue--}

Get or set the flag indicating whether to show the values of the cells on which this data bar is applied. Default value is true.

```javascript
showValue : boolean;
```


### toImage(Cell, ImageOrPrintOptions) {#toImage-cell-imageorprintoptions-}

Render data bar in cell to image byte array.

```javascript
toImage(cell: Cell, imgOpts: ImageOrPrintOptions) : Uint8Array;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| cell | [Cell](../cell/) | Indicate the data bar in which cell to be rendered |
| imgOpts | [ImageOrPrintOptions](../imageorprintoptions/) | ImageOrPrintOptions contains some property of output image |


