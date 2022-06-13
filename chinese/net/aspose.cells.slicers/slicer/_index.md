---
title: Slicer
second_title: Aspose.Cells for .NET API 参考
description: 切片器视图的摘要描述
type: docs
weight: 5630
url: /zh/net/aspose.cells.slicers/slicer/
---
## Slicer class

切片器视图的摘要描述

```csharp
public class Slicer
```

## 特性

| 姓名 | 描述 |
| --- | --- |
| [AlternativeText](../../aspose.cells.slicers/slicer/alternativetext) { get; set; } | 返回或设置切片器对象的描述性（替代）文本字符串。 |
| [Caption](../../aspose.cells.slicers/slicer/caption) { get; set; } | 返回或设置指定切片器的标题。 |
| [CaptionVisible](../../aspose.cells.slicers/slicer/captionvisible) { get; set; } | 返回或设置显示切片器 Caption 的标头是否可见 默认值为 true |
| [ColumnWidth](../../aspose.cells.slicers/slicer/columnwidth) { get; set; } | 返回或设置切片器中每列的宽度（以磅为单位）。 |
| [ColumnWidthPixel](../../aspose.cells.slicers/slicer/columnwidthpixel) { get; set; } | 获取或设置切片器每列的宽度（以像素为单位）。 |
| [Height](../../aspose.cells.slicers/slicer/height) { get; set; } | 返回或设置指定切片器的高度，以磅为单位。 |
| [HeightPixel](../../aspose.cells.slicers/slicer/heightpixel) { get; set; } | 返回或设置指定切片器的高度，以像素为单位。 |
| [IsLocked](../../aspose.cells.slicers/slicer/islocked) { get; set; } | 表示切片器形状是否被锁定。 |
| [IsPrintable](../../aspose.cells.slicers/slicer/isprintable) { get; set; } | 表示切片器对象是否可打印。 |
| [LeftPixel](../../aspose.cells.slicers/slicer/leftpixel) { get; set; } | 返回或设置切片器形状与其左列的水平偏移量，以像素为单位。 |
| [LockedAspectRatio](../../aspose.cells.slicers/slicer/lockedaspectratio) { get; set; } | 表示是否锁定纵横比。 |
| [LockedPosition](../../aspose.cells.slicers/slicer/lockedposition) { get; set; } | 指示是否可以使用用户界面移动或调整指定切片器的大小。 |
| [Name](../../aspose.cells.slicers/slicer/name) { get; set; } | 返回或设置指定切片器的名称 |
| [NumberOfColumns](../../aspose.cells.slicers/slicer/numberofcolumns) { get; set; } | 返回或设置指定切片器中的列数。 |
| [Parent](../../aspose.cells.slicers/slicer/parent) { get; } | 返回表示包含切片器的工作表的 Worksheet 对象。只读。 |
| [Placement](../../aspose.cells.slicers/slicer/placement) { get; set; } | 表示绘图对象附加到它下面的单元格的方式。 该属性控制对象在工作表上的位置。 |
| [RowHeight](../../aspose.cells.slicers/slicer/rowheight) { get; set; } | 返回或设置指定切片器中每一行的高度（以磅为单位）。 |
| [RowHeightPixel](../../aspose.cells.slicers/slicer/rowheightpixel) { get; set; } | 返回或设置指定切片器中每一行的高度（以像素为单位）。 |
| [SlicerCache](../../aspose.cells.slicers/slicer/slicercache) { get; } | 返回与切片器关联的 SlicerCache 对象。只读。 |
| [StyleType](../../aspose.cells.slicers/slicer/styletype) { get; set; } | 指定内置切片器样式的类型 默认类型为 SlicerStyleLight1 |
| [Title](../../aspose.cells.slicers/slicer/title) { get; set; } | 指定当前切片器对象的标题。 |
| [TopPixel](../../aspose.cells.slicers/slicer/toppixel) { get; set; } | 返回或设置切片器形状与其顶行的垂直偏移量，以像素为单位。 |
| [Width](../../aspose.cells.slicers/slicer/width) { get; set; } | 返回或设置指定切片器的宽度，以磅为单位。 |
| [WidthPixel](../../aspose.cells.slicers/slicer/widthpixel) { get; set; } | 返回或设置指定切片器的宽度，以像素为单位。 |

## 方法

| 姓名 | 描述 |
| --- | --- |
| [AddPivotConnection](../../aspose.cells.slicers/slicer/addpivotconnection)(PivotTable) | 添加数据透视表连接。 |
| [Refresh](../../aspose.cells.slicers/slicer/refresh)() | 刷新切片器。同时，刷新和计算相关数据透视表。 |
| [RemovePivotConnection](../../aspose.cells.slicers/slicer/removepivotconnection)(PivotTable) | 删除数据透视表连接。 |

### 例子

```csharp

[C#]

Workbook book = new Workbook();
Worksheet sheet = book.Worksheets[0];
Cells cells = sheet.Cells;
cells[0, 0].Value = "fruit";
cells[1, 0].Value = "grape";
cells[2, 0].Value = "blueberry";
cells[3, 0].Value = "kiwi";
cells[4, 0].Value = "cherry";
cells[5, 0].Value = "grape";
cells[6, 0].Value = "blueberry";
cells[7, 0].Value = "kiwi";
cells[8, 0].Value = "cherry";

cells[0, 1].Value = "year";
cells[1, 1].Value = 2020;
cells[2, 1].Value = 2020;
cells[3, 1].Value = 2020;
cells[4, 1].Value = 2020;
cells[5, 1].Value = 2021;
cells[6, 1].Value = 2021;
cells[7, 1].Value = 2021;
cells[8, 1].Value = 2021;

cells[0, 2].Value = "amount";
cells[1, 2].Value = 50;
cells[2, 2].Value = 60;
cells[3, 2].Value = 70;
cells[4, 2].Value = 80;
cells[5, 2].Value = 90;
cells[6, 2].Value = 100;
cells[7, 2].Value = 110;
cells[8, 2].Value = 120;

PivotTableCollection pivots = sheet.PivotTables;

int pivotIndex = pivots.Add("=Sheet1!A1:C9", "A12", "TestPivotTable");
PivotTable pivot = pivots[pivotIndex];
pivot.AddFieldToArea(PivotFieldType.Row, "fruit");
pivot.AddFieldToArea(PivotFieldType.Column, "year");
pivot.AddFieldToArea(PivotFieldType.Data, "amount");

pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;
pivot.RefreshData();
pivot.CalculateData();

SlicerCollection slicers = sheet.Slicers;
int slicerIndex = slicers.Add(pivot, "E12", "fruit");
Slicer slicer = slicers[slicerIndex];
slicer.StyleType = SlicerStyleType.SlicerStyleLight2;

SlicerCacheItemCollection items = slicer.SlicerCache.SlicerCacheItems;
SlicerCacheItem item = items[0];
item.Selected = false;
 //做你的事
book.Save("out.xlsx");

[Visual Basic]

Dim book As Workbook = New Workbook()
Dim sheet As Worksheet = book.Worksheets(0)
Dim cells As Cells = sheet.Cells

cells(0, 0).Value = "fruit"
cells(1, 0).Value = "grape"
cells(2, 0).Value = "blueberry"
cells(3, 0).Value = "kiwi"
cells(4, 0).Value = "cherry"
cells(5, 0).Value = "grape"
cells(6, 0).Value = "blueberry"
cells(7, 0).Value = "kiwi"
cells(8, 0).Value = "cherry"

cells(0, 1).Value = "year"
cells(1, 1).Value = 2020
cells(2, 1).Value = 2020
cells(3, 1).Value = 2020
cells(4, 1).Value = 2020
cells(5, 1).Value = 2021
cells(6, 1).Value = 2021
cells(7, 1).Value = 2021
cells(8, 1).Value = 2021

cells(0, 2).Value = "amount"
cells(1, 2).Value = 50
cells(2, 2).Value = 60
cells(3, 2).Value = 70
cells(4, 2).Value = 80
cells(5, 2).Value = 90
cells(6, 2).Value = 100
cells(7, 2).Value = 110
cells(8, 2).Value = 120

Dim pivots As PivotTableCollection = sheet.PivotTables
Dim pivotIndex As Int32 = pivots.Add("=Sheet1!A1:C9", "A12", "TestPivotTable")
Dim pivot As PivotTable = pivots(pivotIndex)
pivot.AddFieldToArea(PivotFieldType.Row, "fruit")
Pivot.AddFieldToArea(PivotFieldType.Column, "year")
Pivot.AddFieldToArea(PivotFieldType.Data, "amount")

pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10
pivot.RefreshData()
pivot.CalculateData()

Dim slicers As SlicerCollection = sheet.Slicers
Dim slicerIndex As Int32 = slicers.Add(pivot, "E12", "fruit")
Dim slicer As Slicer = slicers(slicerIndex)
slicer.StyleType = SlicerStyleType.SlicerStyleLight2

Dim items As SlicerCacheItemCollection = slicer.SlicerCache.SlicerCacheItems
Dim item As SlicerCacheItem = items(0)
item.Selected = False

book.Save("out_vb.xlsx")
```

### 也可以看看

* 命名空间 [Aspose.Cells.Slicers](../../aspose.cells.slicers)
* 部件 [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
