---
title: Aspose::Cells::Drawing::Area::SetInvertIfNegative method
linktitle: SetInvertIfNegative
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::Area::SetInvertIfNegative method. If the property is true and the value of chart point is a negative number, the foreground color and background color will be exchanged in C++.'
type: docs
weight: 1300
url: /zh/cpp/aspose.cells.drawing/area/setinvertifnegative/
---
## Area::SetInvertIfNegative method


If the property is true and the value of chart point is a negative number, the foreground color and background color will be exchanged.

```cpp
void Aspose::Cells::Drawing::Area::SetInvertIfNegative(bool value)
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
chart.GetNSeries().Get(0).GetArea().SetInvertIfNegative(true);
//设置第一 NSeries 区域的前景颜色
chart.GetNSeries().Get(0).GetArea().SetForegroundColor(Color{ 0xff, 0xff, 0, 0 });
//Setting the background color of the 1st NSeries area.
//The displayed area color of second chart point will be the background color.
chart.GetNSeries().Get(0).GetArea().SetBackgroundColor(Color{ 0xff, 0xff, 0xff, 0 });
//保存 Excel 文件
workbook.Save(u"book1.xls");

Aspose::Cells::Cleanup();
```

## See Also

* Class [Area](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
