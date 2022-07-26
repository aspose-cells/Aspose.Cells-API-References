---
title: TrendlineCollection
second_title: Aspose.Cells لمرجع .NET API
description: يمثل مجموعة من كافة ملفاتTrendline./trendline كائنات لسلسلة البيانات المحددة.
type: docs
weight: 990
url: /ar/net/aspose.cells.charts/trendlinecollection/
---
## TrendlineCollection class

يمثل مجموعة من كافة ملفات[`Trendline`](../trendline) كائنات لسلسلة البيانات المحددة.

```csharp
public class TrendlineCollection : CollectionBase<Trendline>
```

## الخصائص

| اسم | وصف |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase`1/capacity) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase`1/count) { get; } |  |
| [Item](../../aspose.cells.charts/trendlinecollection/item) { get; } | يحصل على أ الكائن بفهرسها . |
| [Item](../../aspose.cells/collectionbase`1/item) { get; set; } |  |

## طُرق

| اسم | وصف |
| --- | --- |
| [Add](../../aspose.cells.charts/trendlinecollection/add#add)(TrendlineType) | يضيف أ كائن لهذه المجموعة بالنوع المحدد. |
| [Add](../../aspose.cells.charts/trendlinecollection/add#add_1)(TrendlineType, string) | يضيف أ كائن إلى هذه المجموعة بالنوع والاسم المحددين. |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(Trendline) |  |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(Trendline, IComparer&lt;Trendline&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(int, int, Trendline, IComparer&lt;Trendline&gt;) |  |
| [Clear](../../aspose.cells/collectionbase`1/clear)() |  |
| [Contains](../../aspose.cells/collectionbase`1/contains)(Trendline) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(Trendline[]) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(Trendline[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(int, Trendline[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase`1/exists)(Predicate&lt;Trendline&gt;) |  |
| [Find](../../aspose.cells/collectionbase`1/find)(Predicate&lt;Trendline&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase`1/findall)(Predicate&lt;Trendline&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(Predicate&lt;Trendline&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(int, Predicate&lt;Trendline&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(int, int, Predicate&lt;Trendline&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase`1/findlast)(Predicate&lt;Trendline&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(Predicate&lt;Trendline&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(int, Predicate&lt;Trendline&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(int, int, Predicate&lt;Trendline&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase`1/getenumerator)() |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(Trendline) |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(Trendline, int) |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(Trendline, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(Trendline) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(Trendline, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(Trendline, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase`1/removeat)(int) |  |

### أمثلة

```csharp
[C#]

// إنشاء كائن مصنف
Workbook workbook = new Workbook();
// إضافة ورقة عمل جديدة إلى كائن Excel
int sheetIndex = workbook.Worksheets.Add();
// الحصول على مرجع ورقة العمل المضافة حديثًا عن طريق تمرير فهرس الورقة الخاص بها
Worksheet worksheet = workbook.Worksheets[sheetIndex];
worksheet.Cells["A1"].PutValue(50);
worksheet.Cells["A2"].PutValue(100);
worksheet.Cells["A3"].PutValue(150);
worksheet.Cells["A4"].PutValue(200);
worksheet.Cells["B1"].PutValue(60);
worksheet.Cells["B2"].PutValue(32);
worksheet.Cells["B3"].PutValue(50);
worksheet.Cells["B4"].PutValue(40);

// إضافة مخطط إلى ورقة العمل
int chartIndex = workbook.Worksheets[0].Charts.Add(ChartType.Column, 3, 3, 15, 10);
Chart chart = workbook.Worksheets[0].Charts[chartIndex];
chart.NSeries.Add("A1:a3", true);
chart.NSeries[0].TrendLines.Add(TrendlineType.Linear, "MyTrendLine");
Trendline line = chart.NSeries[0].TrendLines[0];
line.DisplayEquation = true;
line.DisplayRSquared = true;
line.Color = Color.Red;

[Visual Basic]

'إنشاء كائن مصنف
Dim workbook As Workbook = New Workbook()
'إضافة ورقة عمل جديدة إلى كائن Excel
Dim sheetIndex As Int32 = workbook.Worksheets.Add()
'الحصول على مرجع ورقة العمل المضافة حديثًا عن طريق تمرير فهرس الورقة الخاص بها
Dim worksheet As Worksheet = workbook.Worksheets(sheetIndex)
worksheet.Cells("A1").PutValue(50)
worksheet.Cells("A2").PutValue(100)
worksheet.Cells("A3").PutValue(150)
worksheet.Cells("A4").PutValue(200)
worksheet.Cells("B1").PutValue(60)
worksheet.Cells("B2").PutValue(32)
worksheet.Cells("B3").PutValue(50)
worksheet.Cells("B4").PutValue(40)

'إضافة مخطط إلى ورقة العمل
Dim chartIndex As Integer =  workbook.Worksheets(0).Charts.Add(ChartType.Column,3,3,15,10) 
Dim chart As Chart =  workbook.Worksheets(0).Charts(chartIndex) 
chart.NSeries.Add("A1:a3", True)
chart.NSeries(0).TrendLines.Add(TrendlineType.Linear, "MyTrendLine")
Dim line As Trendline =  chart.NSeries(0).TrendLines(0) 
line.DisplayEquation = True
line.DisplayRSquared = True
line.Color = Color.Red
```

### أنظر أيضا

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1)
* class [Trendline](../trendline)
* مساحة الاسم [Aspose.Cells.Charts](../../aspose.cells.charts)
* المجسم [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
