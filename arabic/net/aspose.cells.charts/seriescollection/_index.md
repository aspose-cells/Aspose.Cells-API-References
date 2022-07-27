---
title: SeriesCollection
second_title: Aspose.Cells لمرجع .NET API
description: لتغليف مجموعة منSeries./series الكائنات .
type: docs
weight: 830
url: /ar/net/aspose.cells.charts/seriescollection/
---
## SeriesCollection class

لتغليف مجموعة من[`Series`](../series) الكائنات .

```csharp
public class SeriesCollection : CollectionBase<Series>
```

## الخصائص

| اسم | وصف |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase`1/capacity) { get; set; } |  |
| [CategoryData](../../aspose.cells.charts/seriescollection/categorydata) { get; set; } | الحصول على أو تعيين نطاق قيم محور الفئة. يمكن أن يكون نطاقًا من الخلايا (مثل ، "d1: e10") ، أو سلسلة من القيم (مثل ، "{2،6،8،10}"). |
| [Count](../../aspose.cells/collectionbase`1/count) { get; } |  |
| [IsColorVaried](../../aspose.cells.charts/seriescollection/iscolorvaried) { get; set; } | يمثل ما إذا كان لون النقاط متنوعًا. |
| [Item](../../aspose.cells.charts/seriescollection/item) { get; } | يحصل على ملف[`Series`](../series) عنصر في الفهرس المحدد. |
| [Item](../../aspose.cells/collectionbase`1/item) { get; set; } |  |
| [SecondCategoryData](../../aspose.cells.charts/seriescollection/secondcategorydata) { get; set; } | الحصول على أو تعيين نطاق قيم محور الفئة الثانية. يمكن أن يكون نطاقًا من الخلايا (مثل ، "d1: e10") ، أو سلسلة من القيم (مثل ، "{2،6،8،10}"). التأثيرات فقط عندما يتم رسم بعض سلسلة AS على المحور الثاني. |

## طُرق

| اسم | وصف |
| --- | --- |
| [Add](../../aspose.cells.charts/seriescollection/add#add)(string, bool) | يضيف ملف[`SeriesCollection`](../seriescollection) جمع الرسم البياني . |
| [Add](../../aspose.cells.charts/seriescollection/add#add_1)(string, bool, bool) | يضيف ملف[`SeriesCollection`](../seriescollection) جمع الرسم البياني . |
| [AddR1C1](../../aspose.cells.charts/seriescollection/addr1c1)(string, bool) | يضيف ملف[`SeriesCollection`](../seriescollection) جمع الرسم البياني . |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(Series) |  |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(Series, IComparer&lt;Series&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(int, int, Series, IComparer&lt;Series&gt;) |  |
| [ChangeSeriesOrder](../../aspose.cells.charts/seriescollection/changeseriesorder)(int, int) | يغير أوامر السلسلتين مباشرة. |
| [Clear](../../aspose.cells.charts/seriescollection/clear#clear)() | يمسح المجموعة (2 methods) |
| [Contains](../../aspose.cells/collectionbase`1/contains)(Series) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(Series[]) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(Series[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(int, Series[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase`1/exists)(Predicate&lt;Series&gt;) |  |
| [Find](../../aspose.cells/collectionbase`1/find)(Predicate&lt;Series&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase`1/findall)(Predicate&lt;Series&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(Predicate&lt;Series&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(int, Predicate&lt;Series&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(int, int, Predicate&lt;Series&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase`1/findlast)(Predicate&lt;Series&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(Predicate&lt;Series&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(int, Predicate&lt;Series&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(int, int, Predicate&lt;Series&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase`1/getenumerator)() |  |
| [GetSeriesByOrder](../../aspose.cells.charts/seriescollection/getseriesbyorder)(int) | يحصل على ملف[`Series`](../series) عنصر بالترتيب. |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(Series) |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(Series, int) |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(Series, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(Series) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(Series, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(Series, int, int) |  |
| [RemoveAt](../../aspose.cells.charts/seriescollection/removeat#removeat)(int) | إزالة عند سلسلة في الفهرس المحدد . (2 methods) |
| [SetSeriesNames](../../aspose.cells.charts/seriescollection/setseriesnames)(int, string, bool) | يحدد اسم كل السلاسل في الرسم البياني. |

### أمثلة

```csharp

[C#]
// إنشاء كائن مصنف
Workbook workbook = new Workbook();
// إضافة ورقة عمل جديدة إلى كائن Excel
int sheetIndex = workbook.Worksheets.Add();
// الحصول على مرجع ورقة العمل المضافة حديثًا عن طريق تمرير فهرس الورقة الخاص بها
Worksheet worksheet = workbook.Worksheets[sheetIndex];
// إضافة قيمة عينة إلى الخلية "A1"
worksheet.Cells["A1"].PutValue(50);
// إضافة قيمة عينة إلى الخلية "A2"
worksheet.Cells["A2"].PutValue(100);
// إضافة قيمة عينة إلى الخلية "A3"
worksheet.Cells["A3"].PutValue(150);
// إضافة قيمة عينة إلى الخلية "A4"
worksheet.Cells["A4"].PutValue(200);
// إضافة قيمة عينة إلى الخلية "B1"
worksheet.Cells["B1"].PutValue(60);
// إضافة قيمة عينة إلى الخلية "B2"
worksheet.Cells["B2"].PutValue(32);
// إضافة قيمة عينة إلى الخلية "B3"
worksheet.Cells["B3"].PutValue(50);
// إضافة قيمة عينة إلى الخلية "B4"
worksheet.Cells["B4"].PutValue(40);
// إضافة قيمة عينة إلى خلية "C1" كبيانات فئة
worksheet.Cells["C1"].PutValue("Q1");
// إضافة قيمة عينة إلى خلية "C2" كبيانات فئة
worksheet.Cells["C2"].PutValue("Q2");
// إضافة قيمة عينة إلى خلية "C3" كبيانات فئة
worksheet.Cells["C3"].PutValue("Y1");
// إضافة قيمة عينة إلى خلية "C4" كبيانات فئة
worksheet.Cells["C4"].PutValue("Y2");
// إضافة مخطط إلى ورقة العمل
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
// الوصول إلى مثيل المخطط المضاف حديثًا
Chart chart = worksheet.Charts[chartIndex];
// إضافة NSeries (مصدر بيانات المخطط) إلى المخطط الذي يتراوح من خلية "A1" إلى "B4"
chart.NSeries.Add("A1:B4", true);
// تعيين مصدر البيانات لبيانات فئة سلسلة NS
chart.NSeries.CategoryData = "C1:C4";
// حفظ ملف Excel
workbook.Save("book1.xls");

[Visual Basic]

'إنشاء كائن مصنف
Dim workbook As Workbook = New Workbook()
'إضافة ورقة عمل جديدة إلى كائن Excel
Dim sheetIndex As Integer = workbook.Worksheets.Add()
'الحصول على مرجع ورقة العمل المضافة حديثًا عن طريق تمرير فهرس الورقة الخاص بها
Dim worksheet As Worksheet = workbook.Worksheets(sheetIndex)
'Adding a sample value to "A1" cell
worksheet.Cells("A1").PutValue(50)
'Adding a sample value to "A2" cell
worksheet.Cells("A2").PutValue(100)
'Adding a sample value to "A3" cell
worksheet.Cells("A3").PutValue(150)
'Adding a sample value to "A4" cell
worksheet.Cells("A4").PutValue(200)
'Adding a sample value to "B1" cell
worksheet.Cells("B1").PutValue(60)
'Adding a sample value to "B2" cell
worksheet.Cells("B2").PutValue(32)
'Adding a sample value to "B3" cell
worksheet.Cells("B3").PutValue(50)
'Adding a sample value to "B4" cell
worksheet.Cells("B4").PutValue(40)
'Adding a sample value to "C1" cell as category data
worksheet.Cells("C1").PutValue("Q1")
'Adding a sample value to "C2" cell as category data
worksheet.Cells("C2").PutValue("Q2")
'Adding a sample value to "C3" cell as category data
worksheet.Cells("C3").PutValue("Y1")
'Adding a sample value to "C4" cell as category data
worksheet.Cells("C4").PutValue("Y2")
'إضافة مخطط إلى ورقة العمل
Dim chartIndex As Integer = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5)
'الوصول إلى مثيل المخطط المضاف حديثًا
Dim chart As Chart = worksheet.Charts(chartIndex)
'Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B4"
chart.NSeries.Add("A1:B4", True)
'ضبط مصدر البيانات لبيانات فئة NSeries
chart.NSeries.CategoryData = "C1:C4"
'حفظ ملف Excel
workbook.Save("book1.xls")
```

### أنظر أيضا

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1)
* class [Series](../series)
* مساحة الاسم [Aspose.Cells.Charts](../../aspose.cells.charts)
* المجسم [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
