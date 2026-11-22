---
title: "فئة TrendlineCollection"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "فئة Aspose.Cells.Charts.TrendlineCollection. تمثل مجموعة من جميع كائنات Trendline للسلسلة البيانات المحددة"
type: docs
url: /ar/net/aspose.cells.charts/trendlinecollection/
---
## TrendlineCollection class

تمثل مجموعة من جميع كائنات [`Trendline`](../trendline/) للسلسلة البيانات المحددة.

```csharp
public class TrendlineCollection : CollectionBase<Trendline>
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.charts/trendlinecollection/item/) { get; } | يحصل على كائن [`Trendline`](../trendline/) بواسطة فهرسه. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [Add](../../aspose.cells.charts/trendlinecollection/add/#add)(TrendlineType) | يضيف كائن [`Trendline`](../trendline/) إلى هذه المجموعة بالنوع المحدد. |
| [Add](../../aspose.cells.charts/trendlinecollection/add/#add_1)(TrendlineType, string) | يضيف كائن [`Trendline`](../trendline/) إلى هذه المجموعة بالنوع والاسم المحددين. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(Trendline) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(Trendline, IComparer&lt;Trendline&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, Trendline, IComparer&lt;Trendline&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(Trendline) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(Trendline[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(Trendline[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, Trendline[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;Trendline&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;Trendline&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;Trendline&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;Trendline&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;Trendline&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;Trendline&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;Trendline&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;Trendline&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;Trendline&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;Trendline&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Trendline) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Trendline, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Trendline, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Trendline) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Trendline, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Trendline, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;
    using System.Drawing;

    public class TrendlineCollectionDemo
    {
        public static void TrendlineCollectionExample()
        {
            // إنشاء كائن Workbook
            Workbook workbook = new Workbook();
            
            // إضافة ورقة عمل جديدة إلى كائن Excel
            int sheetIndex = workbook.Worksheets.Add();
            
            // الحصول على مرجع ورقة العمل التي تم إضافتها حديثًا بتمرير sheet index
            Worksheet worksheet = workbook.Worksheets[sheetIndex];
            
            // إضافة قيم عينة إلى الخلايا
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
            
            // إضافة NSeries (مصدر بيانات المخطط) إلى المخطط من الخلية "A1" إلى "B4"
            chart.NSeries.Add("A1:A4", true);
            chart.NSeries.Add("B1:B4", true);
            
            // إضافة خط اتجاه إلى السلسلة الأولى
            int trendlineIndex = chart.NSeries[0].TrendLines.Add(TrendlineType.Linear, "MyTrendLine");
            Trendline trendline = chart.NSeries[0].TrendLines[trendlineIndex];
            
            // تعيين خصائص خط الاتجاه
            trendline.DisplayEquation = true;
            trendline.DisplayRSquared = true;
            trendline.Color = Color.Red;

            // حفظ ملف Excel
            workbook.Save("TrendlineCollectionExample.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [Trendline](../trendline/)
* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


