---
title: Aspose::Cells::Charts::SeriesCollection class
linktitle: SeriesCollection
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Charts::SeriesCollection class. Encapsulates a collection of Series objects in C++.'
type: docs
weight: 2600
url: /ar/cpp/aspose.cells.charts/seriescollection/
---
## SeriesCollection class


Encapsulates a collection of [Series](../series/) objects.

```cpp
class SeriesCollection
```

## Methods

| Method | Description |
| --- | --- |
| [Add(const U16String\& dataArea, bool isVertical)](./add/) | Adds the [Series](../series/) collection to a chart. |
| [Add(const char16_t* dataArea, bool isVertical)](./add/) | Adds the [Series](../series/) collection to a chart. |
| [Add(const U16String\& area, bool isVertical, bool checkLabels)](./add/) | Adds the [Series](../series/) collection to a chart. |
| [Add(const char16_t* area, bool isVertical, bool checkLabels)](./add/) | Adds the [Series](../series/) collection to a chart. |
| [AddR1C1(const U16String\& area, bool isVertical)](./addr1c1/) | Adds the [Series](../series/) collection to a chart. |
| [AddR1C1(const char16_t* area, bool isVertical)](./addr1c1/) | Adds the [Series](../series/) collection to a chart. |
| [ChangeColors(ChartColorPaletteType type)](./changecolors/) | Set Monochromatic Palette for chart series. |
| [ChangeSeriesOrder(int32_t sourceIndex, int32_t destIndex)](./changeseriesorder/) |  **(Deprecated)** Directly changes the orders of the two series. |
| [Clear()](./clear/) | Clears the collection. |
| [Get(int32_t index)](./get/) | Gets the [Series](../series/) element at the specified index. |
| [GetCategoryData()](./getcategorydata/) | Gets or sets the range of category [Axis](../axis/) values. It can be a range of cells (such as, "d1:e10"), or a sequence of values (such as,"{2,6,8,10}"). |
| [GetCount()](./getcount/) |  |
| [GetSecondCategoryData()](./getsecondcategorydata/) | Gets or sets the range of second category [Axis](../axis/) values. It can be a range of cells (such as, "d1:e10"), or a sequence of values (such as,"{2,6,8,10}"). Only effects when some series were plotted on the second axis. |
| [GetSeriesByOrder(int32_t order)](./getseriesbyorder/) | Gets the [Series](../series/) element by order. |
| [IsColorVaried()](./iscolorvaried/) | Represents if the color of points is varied. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const SeriesCollection\& src)](./operator_asm/) | operator= |
| [RemoveAt(int32_t index)](./removeat/) | Remove at a series at the specific index. |
| [SeriesCollection(SeriesCollection_Impl* impl)](./seriescollection/) | Constructs from an implementation object. |
| [SeriesCollection(const SeriesCollection\& src)](./seriescollection/) | Copy constructor. |
| [SetCategoryData(const U16String\& value)](./setcategorydata/) | Gets or sets the range of category [Axis](../axis/) values. It can be a range of cells (such as, "d1:e10"), or a sequence of values (such as,"{2,6,8,10}"). |
| [SetCategoryData(const char16_t* value)](./setcategorydata/) | Gets or sets the range of category [Axis](../axis/) values. It can be a range of cells (such as, "d1:e10"), or a sequence of values (such as,"{2,6,8,10}"). |
| [SetIsColorVaried(bool value)](./setiscolorvaried/) | Represents if the color of points is varied. |
| [SetSecondCategoryData(const U16String\& value)](./setsecondcategorydata/) | Gets or sets the range of second category [Axis](../axis/) values. It can be a range of cells (such as, "d1:e10"), or a sequence of values (such as,"{2,6,8,10}"). Only effects when some series were plotted on the second axis. |
| [SetSecondCategoryData(const char16_t* value)](./setsecondcategorydata/) | Gets or sets the range of second category [Axis](../axis/) values. It can be a range of cells (such as, "d1:e10"), or a sequence of values (such as,"{2,6,8,10}"). Only effects when some series were plotted on the second axis. |
| [SetSeriesNames(int32_t startIndex, const U16String\& area, bool isVertical)](./setseriesnames/) | Sets the name of all the serieses in the chart. |
| [SetSeriesNames(int32_t startIndex, const char16_t* area, bool isVertical)](./setseriesnames/) | Sets the name of all the serieses in the chart. |
| [SwapSeries(int32_t sourceIndex, int32_t destIndex)](./swapseries/) | Directly changes the orders of the two series. |
| [~SeriesCollection()](./~seriescollection/) | Destructor. |
## Fields

| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |

## Examples


```cpp
Aspose::Cells::Startup();
//إنشاء كائن Workbook
Workbook workbook;
//إضافة ورقة عمل جديدة إلى كائن Excel
int sheetIndex = workbook.GetWorksheets().Add();
//الحصول على مرجع ورقة العمل المضافة حديثًا بتمرير فهرس الورقة الخاص بها
Worksheet worksheet = workbook.GetWorksheets().Get(sheetIndex);
//إضافة قيمة تجريبية إلى الخلية "A1"
worksheet.GetCells().Get(u"A1").PutValue(50);
//إضافة قيمة تجريبية إلى الخلية "A2"
worksheet.GetCells().Get(u"A2").PutValue(100);
//إضافة قيمة تجريبية إلى الخلية "A3"
worksheet.GetCells().Get(u"A3").PutValue(150);
//إضافة قيمة تجريبية إلى الخلية "A4"
worksheet.GetCells().Get(u"A4").PutValue(200);
//إضافة قيمة تجريبية إلى الخلية "B1"
worksheet.GetCells().Get(u"B1").PutValue(60);
//إضافة قيمة تجريبية إلى الخلية "B2"
worksheet.GetCells().Get(u"B2").PutValue(32);
//إضافة قيمة تجريبية إلى الخلية "B3"
worksheet.GetCells().Get(u"B3").PutValue(50);
//إضافة قيمة تجريبية إلى الخلية "B4"
worksheet.GetCells().Get(u"B4").PutValue(40);
//إضافة قيمة تجريبية إلى الخلية "C1" كبيانات فئة
worksheet.GetCells().Get(u"C1").PutValue(u"Q1");
//إضافة قيمة تجريبية إلى الخلية "C2" كبيانات فئة
worksheet.GetCells().Get(u"C2").PutValue(u"Q2");
//إضافة قيمة تجريبية إلى الخلية "C3" كبيانات فئة
worksheet.GetCells().Get(u"C3").PutValue(u"Y1");
//إضافة قيمة تجريبية إلى الخلية "C4" كبيانات فئة
worksheet.GetCells().Get(u"C4").PutValue(u"Y2");
//إضافة مخطط إلى ورقة العمل
int chartIndex = worksheet.GetCharts().Add(ChartType::Column, 5, 0, 15, 5);
//الوصول إلى نسخة المخطط المضاف حديثًا
Chart chart = worksheet.GetCharts().Get(chartIndex);
//إضافة NSeries (مصدر بيانات المخطط) إلى المخطط من الخلية "A1" إلى "B4"
chart.GetNSeries().Add(u"A1:B4", true);
//تحديد مصدر البيانات لبيانات الفئة الخاصة بـ NSeries
chart.GetNSeries().SetCategoryData(u"C1:C4");
//حفظ ملف Excel
workbook.Save(u"book1.xls");

Aspose::Cells::Cleanup();
```

## See Also

* Namespace [Aspose::Cells::Charts](../)
* Library [Aspose.Cells for C++](../../)
