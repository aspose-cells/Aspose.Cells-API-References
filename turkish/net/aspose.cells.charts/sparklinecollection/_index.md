---
title: "Sınıf SparklineCollection"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Charts.SparklineCollection class. Sparkline nesnelerinin bir koleksiyonunu kapsar."
type: docs
url: /tr/net/aspose.cells.charts/sparklinecollection/
---
## SparklineCollection class

[`Sparkline`](../sparkline/) nesnelerinin bir koleksiyonunu kapsar.

```csharp
public class SparklineCollection : CollectionBase<Sparkline>
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.charts/sparklinecollection/item/) { get; } | Belirtilen indeksteki [`Sparkline`](../sparkline/) öğesini alır. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [Add](../../aspose.cells.charts/sparklinecollection/add/)(string, int, int) | Bir sparkline ekle. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(Sparkline) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(Sparkline, IComparer&lt;Sparkline&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, Sparkline, IComparer&lt;Sparkline&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(Sparkline) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(Sparkline[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(Sparkline[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, Sparkline[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;Sparkline&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;Sparkline&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;Sparkline&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;Sparkline&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;Sparkline&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;Sparkline&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;Sparkline&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;Sparkline&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;Sparkline&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;Sparkline&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Sparkline) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Sparkline, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Sparkline, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Sparkline) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Sparkline, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Sparkline, int, int) |  |
| [Remove](../../aspose.cells.charts/sparklinecollection/remove/)(object) | (**Obsolete.**) Sparkline'ı kaldırır |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |
| [RemoveSparkline](../../aspose.cells.charts/sparklinecollection/removesparkline/)(Sparkline) | Sparkline'ı kaldırır |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class SparklineCollectionDemo
    {
        public static void SparklineCollectionExample()
        {
            // Yeni bir çalışma kitabı oluşturun ve ilk çalışma sayfasını alın.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına örnek veri ekle
            worksheet.Cells["A1"].PutValue(5);
            worksheet.Cells["B1"].PutValue(2);
            worksheet.Cells["C1"].PutValue(1);
            worksheet.Cells["D1"].PutValue(3);
            

            // Sparklineların ekleneceği CellArea'ı tanımla
            CellArea cellArea = new CellArea { StartColumn = 4, EndColumn = 4, StartRow = 0, EndRow = 0 };

            // Çalışma sayfasına yeni bir SparklineGroup ekle
            int sparklineGroupIndex = worksheet.SparklineGroups.Add(SparklineType.Line, "A1:D1", false, cellArea);
            SparklineGroup sparklineGroup = worksheet.SparklineGroups[sparklineGroupIndex];

            SparklineCollection sparklineCollection = sparklineGroup.Sparklines;
            Console.WriteLine("Sparkline count: " + sparklineCollection.Count);

            // SparklineGroup'a sparklinelar ekle
            sparklineCollection.Add("A1:D1", 0, 5);

            Console.WriteLine("Sparkline count: " + sparklineCollection.Count);

            // SparklineGroup için çeşitli özellikleri ayarla
            sparklineGroup.ShowHighPoint = true;
            sparklineGroup.ShowLowPoint = true;

            // Yüksek ve düşük noktalar için renkleri ayarla
            CellsColor highPointColor = workbook.CreateCellsColor();
            highPointColor.Color = System.Drawing.Color.Green;
            sparklineGroup.HighPointColor = highPointColor;

            CellsColor lowPointColor = workbook.CreateCellsColor();
            lowPointColor.Color = System.Drawing.Color.Red;
            sparklineGroup.LowPointColor = lowPointColor;

            // Seri rengini ve çizgi kalınlığını ayarla
            CellsColor seriesColor = workbook.CreateCellsColor();
            seriesColor.Color = System.Drawing.Color.Orange;
            sparklineGroup.SeriesColor = seriesColor;
            sparklineGroup.LineWeight = 1.0;

            // Çalışma kitabını kaydedin
            workbook.Save("SparklineCollectionExample.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [Sparkline](../sparkline/)
* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


