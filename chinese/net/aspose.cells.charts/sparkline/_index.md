---
title: Sparkline
second_title: Aspose.Cells for .NET API 参考
description: 迷你图表示工作表单元格中的小图表或图形提供数据的可视化表示
type: docs
weight: 850
url: /zh/net/aspose.cells.charts/sparkline/
---
## Sparkline class

迷你图表示工作表单元格中的小图表或图形，提供数据的可视化表示。

```csharp
[C#]
 Workbook book = new Workbook(); 
 Worksheet sheet = book.Worksheets[0];

 sheet.Cells["A1"].PutValue(5);
 sheet.Cells["B1"].PutValue(2);
 sheet.Cells["C1"].PutValue(1);
 sheet.Cells["D1"].PutValue(3);
 
 // 定义单元格区域
 CellArea ca = new CellArea();
 ca.StartColumn = 4;
 ca.EndColumn = 4;
 ca.StartRow = 0;
 ca.EndRow = 0;

 int idx = sheet.SparklineGroupCollection.Add(Aspose.Cells.Charts.SparklineType.Line, sheet.Name + "!A1:D1", false, ca);

 SparklineGroup group = sheet.SparklineGroupCollection[idx];
 idx = group.SparklineCollection.Add(sheet.Name + "!A1:D1", 0, 4);
 Sparkline line = group.SparklineCollection[idx];
 Console.WriteLine($"Saprkline data range:{line.DataRange}, row:{line.Row}, column:{line.Column}");
 line.ToImage("output.png", new ImageOrPrintOptions());
```

```csharp
public class Sparkline
```

## 特性

| 姓名 | 描述 |
| --- | --- |
| [Column](../../aspose.cells.charts/sparkline/column) { get; } | 获取迷你图的列索引。 |
| [DataRange](../../aspose.cells.charts/sparkline/datarange) { get; set; } | 代表迷你图的数据范围。 |
| [Row](../../aspose.cells.charts/sparkline/row) { get; } | 获取迷你图的行索引。 |

## 方法

| 姓名 | 描述 |
| --- | --- |
| [ToImage](../../aspose.cells.charts/sparkline/toimage#toimage)(ImageOrPrintOptions) | 将迷你图转换为图像。 |
| [ToImage](../../aspose.cells.charts/sparkline/toimage#toimage_1)(Stream, ImageOrPrintOptions) | 将迷你图转换为图像。 |
| [ToImage](../../aspose.cells.charts/sparkline/toimage#toimage_2)(string, ImageOrPrintOptions) | 将迷你图转换为图像。 |

### 也可以看看

* 命名空间 [Aspose.Cells.Charts](../../aspose.cells.charts)
* 部件 [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
