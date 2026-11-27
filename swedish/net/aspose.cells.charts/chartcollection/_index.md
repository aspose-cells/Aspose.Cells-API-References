---
title: "Klass ChartCollection"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Charts.ChartCollection-klass. Inkapslar en samling av Chart-objekt"
type: docs
url: /sv/net/aspose.cells.charts/chartcollection/
---
## ChartCollection class

Inkapslar en samling av [`Chart`](../chart/) objekt.

```csharp
public class ChartCollection : CollectionBase<Chart>
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.charts/chartcollection/item/) { get; } | Hämtar [`Chart`](../chart/) elementet på det angivna indexet. (2 indexerare) |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [Add](../../aspose.cells.charts/chartcollection/add/#add)(ChartType, int, int, int, int) | Lägger till ett diagram i samlingen. |
| [Add](../../aspose.cells.charts/chartcollection/add/#add_2)(ChartType, string, int, int, int, int) | (**Obsolete.**) Lägger till ett diagram i samlingen. |
| [Add](../../aspose.cells.charts/chartcollection/add/#add_3)(byte[], string, bool, int, int, int, int) | Lägger till ett diagram med förinställd mall. |
| [Add](../../aspose.cells.charts/chartcollection/add/#add_1)(ChartType, string, bool, int, int, int, int) | Lägger till ett diagram i samlingen. |
| [AddFloatingChart](../../aspose.cells.charts/chartcollection/addfloatingchart/)(ChartType, int, int, int, int) | Lägger till ett diagram i samlingen. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(Chart) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(Chart, IComparer&lt;Chart&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, Chart, IComparer&lt;Chart&gt;) |  |
| [Clear](../../aspose.cells.charts/chartcollection/clear/#clear)() | Rensa alla diagram. (2 metoder) |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(Chart) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(Chart[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(Chart[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, Chart[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;Chart&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;Chart&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;Chart&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;Chart&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;Chart&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;Chart&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;Chart&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;Chart&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;Chart&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;Chart&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Chart) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Chart, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Chart, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Chart) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Chart, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Chart, int, int) |  |
| [RemoveAt](../../aspose.cells.charts/chartcollection/removeat/#removeat)(int) | Ta bort ett diagram på det specifika indexet. (2 metoder) |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartCollectionDemo
    {
        public static void ChartCollectionExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till lite exempeldata i kalkylbladet
            worksheet.Cells[0, 0].PutValue("Category");
            worksheet.Cells[0, 1].PutValue("Value");
            worksheet.Cells[1, 0].PutValue("A");
            worksheet.Cells[1, 1].PutValue(10);
            worksheet.Cells[2, 0].PutValue("B");
            worksheet.Cells[2, 1].PutValue(20);
            worksheet.Cells[3, 0].PutValue("C");
            worksheet.Cells[3, 1].PutValue(30);

            // Åtkomst till diagramsamlingen i kalkylbladet
            ChartCollection charts = worksheet.Charts;

            // Lägg till ett diagram i kalkylbladet
            int chartIndex = charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = charts[chartIndex];

            // Ange dataintervallet för diagrammet
            chart.SetChartDataRange("A1:B4", true);

            // Anpassa diagrammet
            chart.Title.Text = "Sample Chart";
            chart.ShowLegend = true;

            // Spara arbetsboken
            workbook.Save("ChartCollectionExample.xlsx");
            workbook.Save("ChartCollectionExample.pdf");
        }
    }
}
```

### Se även

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [Chart](../chart/)
* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


