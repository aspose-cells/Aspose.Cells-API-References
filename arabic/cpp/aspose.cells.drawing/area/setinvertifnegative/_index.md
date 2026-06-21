---
title: Aspose::Cells::Drawing::Area::SetInvertIfNegative method
linktitle: SetInvertIfNegative
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::Area::SetInvertIfNegative method. If the property is true and the value of chart point is a negative number, the foreground color and background color will be exchanged in C++.'
type: docs
weight: 1300
url: /ar/cpp/aspose.cells.drawing/area/setinvertifnegative/
---
## Area::SetInvertIfNegative method


If the property is true and the value of chart point is a negative number, the foreground color and background color will be exchanged.

```cpp
void Aspose::Cells::Drawing::Area::SetInvertIfNegative(bool value)
```


## Examples


```cpp
Aspose::Cells::Startup();
//إنشاء كائن Workbook
Workbook workbook;
//إضافة ورقة عمل جديدة إلى كائن Workbook
int sheetIndex = workbook.GetWorksheets().Add();
//الحصول على مرجع ورقة العمل المضافة حديثًا بتمرير فهرس الورقة الخاص بها
Worksheet worksheet = workbook.GetWorksheets().Get(sheetIndex);
//إضافة قيمة تجريبية إلى الخلية "A1"
worksheet.GetCells().Get(u"A1").PutValue(50);
//إضافة قيمة تجريبية إلى الخلية "A2"
worksheet.GetCells().Get(u"A2").PutValue(-100);
//إضافة قيمة تجريبية إلى الخلية "A3"
worksheet.GetCells().Get(u"A3").PutValue(150);
//إضافة مخطط إلى ورقة العمل
int chartIndex = worksheet.GetCharts().Add(ChartType::Column, 5, 0, 15, 5);
//الوصول إلى نسخة المخطط المضاف حديثًا
Chart chart = worksheet.GetCharts().Get(chartIndex);
//إضافة NSeries (مصدر بيانات المخطط) إلى المخطط من الخلية "A1" إلى الخلية "A3"
chart.GetNSeries().Add(u"A1:A3", true);
chart.GetNSeries().Get(0).GetArea().SetInvertIfNegative(true);
//Setting the foreground color of the 1st NSeries area
chart.GetNSeries().Get(0).GetArea().SetForegroundColor(Color{ 0xff, 0xff, 0, 0 });
//تعيين لون الخلفية لمنطقة NSeries الأولى.
//سيكون لون المنطقة المعروضة للنقطة الثانية في المخطط هو لون الخلفية.
chart.GetNSeries().Get(0).GetArea().SetBackgroundColor(Color{ 0xff, 0xff, 0xff, 0 });
//حفظ ملف Excel
workbook.Save(u"book1.xls");

Aspose::Cells::Cleanup();
```

## See Also

* Class [Area](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
