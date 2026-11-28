---
title: "Sınıf SparklineGroupCollection"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Charts.SparklineGroupCollection sınıfı. SparklineGroup nesnelerinin bir koleksiyonunu kapsar."
type: docs
url: /tr/net/aspose.cells.charts/sparklinegroupcollection/
---
## SparklineGroupCollection class

[`SparklineGroup`](../sparklinegroup/) nesnelerinin bir koleksiyonunu kapsar.

```csharp
public class SparklineGroupCollection : CollectionBase<SparklineGroup>
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.charts/sparklinegroupcollection/item/) { get; } | Belirtilen indeksteki [`SparklineGroup`](../sparklinegroup/) öğesini alır. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [Add](../../aspose.cells.charts/sparklinegroupcollection/add/#add)(SparklineType) | Koleksiyona bir [`Sparkline`](../sparkline/) içeren bir [`SparklineGroup`](../sparklinegroup/) ekler. |
| [Add](../../aspose.cells.charts/sparklinegroupcollection/add/#add_1)(SparklineType, string, bool, CellArea) | Koleksiyona bazı [`Sparkline`](../sparkline/) içeren bir [`SparklineGroup`](../sparklinegroup/) ekler. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(SparklineGroup) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(SparklineGroup, IComparer&lt;SparklineGroup&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, SparklineGroup, IComparer&lt;SparklineGroup&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [ClearSparklineGroups](../../aspose.cells.charts/sparklinegroupcollection/clearsparklinegroups/)(CellArea) | Hücre alanıyla çakışan sparkline gruplarını temizler. |
| [ClearSparklines](../../aspose.cells.charts/sparklinegroupcollection/clearsparklines/)(CellArea) | Hücre alanı içinde bulunan sparklineları temizler. |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(SparklineGroup) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(SparklineGroup[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(SparklineGroup[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, SparklineGroup[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;SparklineGroup&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;SparklineGroup&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;SparklineGroup&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;SparklineGroup&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;SparklineGroup&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;SparklineGroup&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;SparklineGroup&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;SparklineGroup&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;SparklineGroup&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;SparklineGroup&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(SparklineGroup) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(SparklineGroup, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(SparklineGroup, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(SparklineGroup) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(SparklineGroup, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(SparklineGroup, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;
    using System.Drawing;

    public class SparklineGroupCollectionDemo
    {
        public static void SparklineGroupCollectionExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Çalışma sayfasına bazı veriler ekle
            sheet.Cells["A1"].PutValue(5);
            sheet.Cells["B1"].PutValue(2);
            sheet.Cells["C1"].PutValue(1);
            sheet.Cells["D1"].PutValue(3);

            // Sparkline için CellArea'yı tanımla
            CellArea ca = new CellArea
            {
                StartColumn = 4,
                EndColumn = 4,
                StartRow = 0,
                EndRow = 0
            };

            // Çalışma sayfasına bir sparkline grubu ekle
            int idx = sheet.SparklineGroups.Add(SparklineType.Line, "A1:D1", false, ca);
            SparklineGroup group = sheet.SparklineGroups[idx];

            // Gruba sparkline'lar ekle
            group.Sparklines.Add(sheet.Name + "!A1:D1", 0, 5);

            // Kıvırcık grafik grubunu özelleştir
            group.ShowHighPoint = true;
            group.ShowLowPoint = true;
            group.HighPointColor.Color = Color.Green;
            group.LowPointColor.Color = Color.Red;
            group.LineWeight = 1.0;

            // Çalışma kitabını kaydedin
            workbook.Save("SparklineGroupCollectionExample.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ayrıca Bakınız

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [SparklineGroup](../sparklinegroup/)
* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


