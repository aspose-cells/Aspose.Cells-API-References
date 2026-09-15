---
title: Aspose::Cells::Drawing::Area::GetInvertIfNegative method
linktitle: GetInvertIfNegative
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::Area::GetInvertIfNegative method. If the property is true and the value of chart point is a negative number, the foreground color and background color will be exchanged in C++.'
type: docs
weight: 1200
url: /zh/cpp/aspose.cells.drawing/area/getinvertifnegative/
---
## Area::GetInvertIfNegative method


If the property is true and the value of chart point is a negative number, the foreground color and background color will be exchanged.

```cpp
bool Aspose::Cells::Drawing::Area::GetInvertIfNegative()
```


## Examples


```cpp
Aspose::Cells::Startup();
//实例化 Workbook 对象
Workbook workbook;
//向 Workbook 对象添加新工作表
int sheetIndex = workbook.GetWorksheets().Add();
//通过传递工作表索引获取新添加工作表的引用
Worksheet worksheet = workbook.GetWorksheets().Get(sheetIndex);
//向 "A1" 单元格添加示例值
worksheet.GetCells().Get(u"A1").PutValue(50);
//向 "A2" 单元格添加示例值
worksheet.GetCells().Get(u"A2").PutValue(-100);
//向 "A3" 单元格添加示例值
worksheet.GetCells().Get(u"A3").PutValue(150);
//向工作表添加图表
int chartIndex = worksheet.GetCharts().Add(ChartType::Column, 5, 0, 15, 5);
//访问新添加图表的实例
Chart chart = worksheet.GetCharts().Get(chartIndex);
//Adding NSeries (chart data source) to the chart ranging from "A1" cell to "A3"
chart.GetNSeries().Add(u"A1:A3", true);
bool isNegative = chart.GetNSeries().Get(0).GetArea().GetInvertIfNegative();
Aspose::Cells::Cleanup();
```

## See Also

* Class [Area](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
