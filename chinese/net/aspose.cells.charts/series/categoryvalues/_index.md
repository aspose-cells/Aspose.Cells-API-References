---
title: "Series.CategoryValues"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Series 属性。获取用于在图表中绘制此系列每个点的实际类别值"
type: docs
url: /zh/net/aspose.cells.charts/series/categoryvalues/
---
## Series.CategoryValues property

获取用于在图表中绘制此系列每个点的实际类别值。

```csharp
public ChartDataValue[][] CategoryValues { get; }
```

### 备注

此属性提供了一种便捷方式来获取由[`XValues`](../xvalues/)定义的数据对应的实际值，尤其是当指定的数据源是外部链接、公式等时。

### 示例

```csharp
//演示展示需要此属性的一个案例：
[C#]

//独立示例
Workbook workbook = new Workbook("ExternalSourceChart.xlsx");
Worksheet worksheet = workbook.Worksheets[0];
Chart chart = worksheet.Charts[0];
chart.Calculate();
string XValues = chart.NSeries[0].XValues;
// XValues 可能类似于 "[External.xlsx]Sheet1!$B$2:$C$6"，这比较复杂
// 供用户获取实际值（这些值可能链接到另一个工作簿，
// 或缓存于当前工作簿中)。这里可以使用 CategoryValues 属性
// 以获取在 Excel 界面中实际显示的类别值
// 以二维数组的形式。
ChartDataValue[][] v1 = chart.NSeries[0].CategoryValues;

```

### 另请参见

* class [ChartDataValue](../../chartdatavalue/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


