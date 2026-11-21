---
title: Area
second_title: Aspose.Cells for JavaScript via C++ API Reference
description: Encapsulates the object that represents an area format.
type: docs
url: /zh/javascript-cpp/area/
---

## Area class

Encapsulates the object that represents an area format.

```javascript
class Area;
```


### Example
```javascript
const { Workbook, ChartType, Color, SaveFormat } = AsposeCells;

//实例化一个 Workbook 对象
var workbook = new Workbook();
//向 Workbook 对象添加新工作表
var sheetIndex = workbook.worksheets.add();
//通过传递工作表索引获取新添加工作表的引用
var worksheet = workbook.worksheets.get(sheetIndex);
//向 "A1" 单元格添加示例值
worksheet.cells.get("A1").putValue(50);
//向 "A2" 单元格添加示例值
worksheet.cells.get("A2").putValue(100);
//向 "A3" 单元格添加示例值
worksheet.cells.get("A3").putValue(150);
//向 "B1" 单元格添加示例值
worksheet.cells.get("B1").putValue(60);
//向 "B2" 单元格添加示例值
worksheet.cells.get("B2").putValue(32);
//向 "B3" 单元格添加示例值
worksheet.cells.get("B3").putValue(50);
//向工作表添加图表
var chartIndex = worksheet.charts.add(ChartType.Column, 5, 0, 15, 5);
//访问新添加图表的实例
var chart = worksheet.charts.get(chartIndex);
//向图表添加 NSeries（图表数据源），范围从 "A1" 单元格到 "B3"
chart.nSeries.add("A1:B3", true);
//设置绘图区域的前景色
chart.plotArea.getArea().foregroundColor = Color.Blue;
//设置图表区域的前景色
chart.chartArea.getArea().foregroundColor = Color.Yellow;
//设置第一个 NSeries 区域的前景色
chart.nSeries.get(0).area.foregroundColor = Color.Red;
//设置第一个 NSeries 点区域的前景色
chart.nSeries.get(0).points.get(0).area.foregroundColor = Color.Cyan;
//保存 Excel 文件
var uint8Array = workbook.save(SaveFormat.Excel97To2003);
```
## Properties

| Property | Type | Description |
| --- | --- | --- |
| [backgroundColor](#backgroundColor--)| Color | Gets or sets the background [Color](../color/) of the [Area](../area/). |
| [foregroundColor](#foregroundColor--)| Color | Gets or sets the foreground [Color](../color/). |
| [formatting](#formatting--)| FormattingType | Represents the formatting of the area. |
| [invertIfNegative](#invertIfNegative--)| boolean | If the property is true and the value of chart point is a negative number, the foreground color and background color will be exchanged. |
| [fillFormat](#fillFormat--)| FillFormat | Readonly. Represents a [FillFormat](../fillformat/) object that contains fill formatting properties for the specified chart or shape. |
| [transparency](#transparency--)| number | Returns or sets the degree of transparency of the area as a value from 0.0 (opaque) through 1.0 (clear). |


### backgroundColor {#backgroundColor--}

Gets or sets the background [Color](../color/) of the [Area](../area/).

```javascript
backgroundColor : Color;
```


### foregroundColor {#foregroundColor--}

Gets or sets the foreground [Color](../color/).

```javascript
foregroundColor : Color;
```


### formatting {#formatting--}

Represents the formatting of the area.

```javascript
formatting : FormattingType;
```


### invertIfNegative {#invertIfNegative--}

If the property is true and the value of chart point is a negative number, the foreground color and background color will be exchanged.

```javascript
invertIfNegative : boolean;
```


**Example**
```javascript
const { Workbook, ChartType, Color, SaveFormat } = AsposeCells;

//实例化一个 Workbook 对象
var workbook = new Workbook();
//向 Workbook 对象添加新工作表
var sheetIndex = workbook.worksheets.add();
//通过传递工作表索引获取新添加工作表的引用
var worksheet = workbook.worksheets.get(sheetIndex);
//向 "A1" 单元格添加示例值
worksheet.cells.get("A1").putValue(50);
//向 "A2" 单元格添加示例值
worksheet.cells.get("A2").putValue(-100);
//向 "A3" 单元格添加示例值
worksheet.cells.get("A3").putValue(150);
//向工作表添加图表
var chartIndex = worksheet.charts.add(ChartType.Column, 5, 0, 15, 5);
//访问新添加图表的实例
var chart = worksheet.charts.get(chartIndex);
//将 NSeries（图表数据源）添加到从 "A1" 单元格到 "A3" 的图表中
chart.nSeries.add("A1:A3", true);
chart.nSeries.get(0).area.invertIfNegative = true;
//设置第一个 NSeries 区域的前景色
chart.nSeries.get(0).area.foregroundColor = Color.Red;
//设置第一个 NSeries 区域的背景色。
//第二个图表点显示的区域颜色将为背景色。
chart.nSeries.get(0).area.backgroundColor = Color.Yellow;
//保存 Excel 文件
var uint8Array = workbook.save(SaveFormat.Excel97To2003);
```

### fillFormat {#fillFormat--}

Readonly. Represents a [FillFormat](../fillformat/) object that contains fill formatting properties for the specified chart or shape.

```javascript
fillFormat : FillFormat;
```


### transparency {#transparency--}

Returns or sets the degree of transparency of the area as a value from 0.0 (opaque) through 1.0 (clear).

```javascript
transparency : number;
```



