---
title: "Series.PointValues"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Series 属性。获取用于在图表中绘制此系列每个点的实际值"
type: docs
url: /zh/net/aspose.cells.charts/series/pointvalues/
---
## Series.PointValues property

获取用于在图表中绘制此系列每个点的实际值。

```csharp
public ChartDataValue[] PointValues { get; }
```

### 备注

此属性提供了一种便捷方式来获取由 [`Values`](../values/) 定义的数据对应的实际值，尤其是在指定的数据源是外部链接、公式等情况下。

### 示例

```csharp
//演示展示需要此属性的一个案例：
[C#]

Workbook workbook = new Workbook("ExternalSourceChart.xlsx");
Worksheet worksheet = workbook.Worksheets[0];
Chart chart = worksheet.Charts[0];
chart.Calculate();
string Values = chart.NSeries[0].Values;
// Values 可能类似于 "[External.xlsx]Sheet1!$A$1:$A$6"，这比较复杂
// 供用户获取实际值（这些值可能链接到另一个工作簿，
// 或缓存于当前工作簿）。此处可使用 PointValues 属性
// 以获取在 Excel 界面中实际显示的值
// 以数组形式。
ChartDataValue[] v1 = chart.NSeries[0].PointValues;

```

### 另请参见

* class [ChartDataValue](../../chartdatavalue/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


