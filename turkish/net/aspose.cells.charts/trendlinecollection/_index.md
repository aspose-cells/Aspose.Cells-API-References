---
title: "Sınıf TrendlineCollection"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Charts.TrendlineCollection sınıfı. Belirtilen veri serisi için tüm Trendline nesnelerinin bir koleksiyonunu temsil eder"
type: docs
url: /tr/net/aspose.cells.charts/trendlinecollection/
---
## TrendlineCollection class

Belirtilen veri serisi için tüm [`Trendline`](../trendline/) nesnelerinin bir koleksiyonunu temsil eder.

```csharp
public class TrendlineCollection : CollectionBase<Trendline>
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.charts/trendlinecollection/item/) { get; } | Bir [`Trendline`](../trendline/) nesnesini diziniyle alır. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [Add](../../aspose.cells.charts/trendlinecollection/add/#add)(TrendlineType) | Belirtilen türle bu koleksiyona bir [`Trendline`](../trendline/) nesnesi ekler. |
| [Add](../../aspose.cells.charts/trendlinecollection/add/#add_1)(TrendlineType, string) | Belirtilen tür ve adla bu koleksiyona bir [`Trendline`](../trendline/) nesnesi ekler. |
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

### Örnekler

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
            // Workbook nesnesi örnekleniyor
            Workbook workbook = new Workbook();
            
            // Excel nesnesine yeni bir çalışma sayfası ekleme
            int sheetIndex = workbook.Worksheets.Add();
            
            // Eklenen yeni çalışma sayfasının referansını, sayfa indeksini geçirerek elde etme
            Worksheet worksheet = workbook.Worksheets[sheetIndex];
            
            // Hücrelere örnek değerler ekleme
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["A4"].PutValue(200);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);
            worksheet.Cells["B4"].PutValue(40);

            // Çalışma sayfasına bir grafik ekleme
            int chartIndex = workbook.Worksheets[0].Charts.Add(ChartType.Column, 3, 3, 15, 10);
            Chart chart = workbook.Worksheets[0].Charts[chartIndex];
            
            // Grafiğe, "A1" hücresinden "B4" hücresine kadar olan NSeries (grafik veri kaynağı) ekleme.
            chart.NSeries.Add("A1:A4", true);
            chart.NSeries.Add("B1:B4", true);
            
            // İlk seriye bir trend çizgisi ekleme
            int trendlineIndex = chart.NSeries[0].TrendLines.Add(TrendlineType.Linear, "MyTrendLine");
            Trendline trendline = chart.NSeries[0].TrendLines[trendlineIndex];
            
            // Trend çizgisi özelliklerini ayarlama
            trendline.DisplayEquation = true;
            trendline.DisplayRSquared = true;
            trendline.Color = Color.Red;

            // Excel dosyasını kaydetme
            workbook.Save("TrendlineCollectionExample.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [Trendline](../trendline/)
* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


