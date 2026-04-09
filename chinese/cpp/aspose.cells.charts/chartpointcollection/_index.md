---
title: Aspose::Cells::Charts::ChartPointCollection class
linktitle: ChartPointCollection
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Charts::ChartPointCollection class. Represents a collection that contains all the points in one series in C++.'
type: docs
weight: 1100
url: /zh/cpp/aspose.cells.charts/chartpointcollection/
---
## ChartPointCollection class


Represents a collection that contains all the points in one series.

```cpp
class ChartPointCollection
```

## Methods

| Method | Description |
| --- | --- |
| [ChartPointCollection(ChartPointCollection_Impl* impl)](./chartpointcollection/) | Constructs from an implementation object. |
| [ChartPointCollection(const ChartPointCollection\& src)](./chartpointcollection/) | Copy constructor. |
| [Clear()](./clear/) | Remove all setting of the chart points. |
| [Get(int32_t index)](./get/) | Gets the [ChartPoint](../chartpoint/) element at the specified index in the series. |
| [GetCount()](./getcount/) | Gets the count of the chart point. |
| [GetEnumerator()](./getenumerator/) | Returns an enumerator for the entire [ChartPointCollection](./). |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const ChartPointCollection\& src)](./operator_asm/) | operator= |
| [RemoveAt(int32_t index)](./removeat/) | Removes point at the index of the series.. |
| [~ChartPointCollection()](./~chartpointcollection/) | Destructor. |
## Fields

| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |

## Examples


```cpp
Aspose::Cells::Startup();
//实例化 Workbook 对象
Workbook workbook;

//获取第一个工作表的引用
Worksheet worksheet = workbook.GetWorksheets().Get(0);

//向 "A1" 单元格添加示例值
worksheet.GetCells().Get(u"A1").PutValue(50);

//向 "A2" 单元格添加示例值
worksheet.GetCells().Get(u"A2").PutValue(100);

//向 "A3" 单元格添加示例值
worksheet.GetCells().Get(u"A3").PutValue(150);

//向 "B1" 单元格添加示例值
worksheet.GetCells().Get(u"B1").PutValue(60);

//向 "B2" 单元格添加示例值
worksheet.GetCells().Get(u"B2").PutValue(32);

//向 "B3" 单元格添加示例值
worksheet.GetCells().Get(u"B3").PutValue(50);

//向工作表添加图表
int chartIndex = worksheet.GetCharts().Add(ChartType::PieExploded, 5, 0, 25, 10);

//访问新添加图表的实例
Chart chart = worksheet.GetCharts().Get(chartIndex);

//将 NSeries（图表数据源）添加到图表，范围从 "A1" 单元格到 "B3"
chart.GetNSeries().Add(u"A1:B3", true);

//显示数据标签
chart.GetNSeries().Get(0).GetDataLabels().SetShowValue(true);

ChartPointCollection points = chart.GetNSeries().Get(0).GetPoints();

for (int i = 0; i < points.GetCount(); i++)
{
    //获取数据点
    ChartPoint point = points.Get(i);
    //设置 Pir 爆炸
    point.SetExplosion(15);
    //设置边框颜色
    point.GetBorder().SetColor(Color{ 0xff, 0xff, 0, 0 });
}

//保存 Excel 文件
workbook.Save(u"book1.xls");

Aspose::Cells::Cleanup();
```

## See Also

* Namespace [Aspose::Cells::Charts](../)
* Library [Aspose.Cells for C++](../../)
