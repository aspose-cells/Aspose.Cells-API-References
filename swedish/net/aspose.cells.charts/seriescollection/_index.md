---
title: "Klass SeriesCollection"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Charts.SeriesCollection-klass. Inkapslar en samling av Series‑objekt"
type: docs
url: /sv/net/aspose.cells.charts/seriescollection/
---
## SeriesCollection class

Inkapslar en samling av [`Series`](../series/)‑objekt.

```csharp
public class SeriesCollection : CollectionBase<Series>
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [CategoryData](../../aspose.cells.charts/seriescollection/categorydata/) { get; set; } | Hämtar eller anger intervallet för kategori‑axelvärden. Det kan vara ett cellintervall (t.ex. "d1:e10") eller en sekvens av värden (t.ex. "{2,6,8,10}"). |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [IsColorVaried](../../aspose.cells.charts/seriescollection/iscolorvaried/) { get; set; } | Representerar om färgen på punkterna varierar. |
| [Item](../../aspose.cells.charts/seriescollection/item/) { get; } | Hämtar [`Series`](../series/)‑elementet på det angivna indexet. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |
| [SecondCategoryData](../../aspose.cells.charts/seriescollection/secondcategorydata/) { get; set; } | Hämtar eller anger intervallet för den andra kategori‑axelns värden. Det kan vara ett cellintervall (t.ex. "d1:e10") eller en sekvens av värden (t.ex. "{2,6,8,10}"). Påverkar endast när vissa serier har plottats på den andra axeln. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [Add](../../aspose.cells.charts/seriescollection/add/#add)(string, bool) | Lägger till [`Series`](../series/)‑samlingen i ett diagram. |
| [Add](../../aspose.cells.charts/seriescollection/add/#add_1)(string, bool, bool) | Lägger till [`Series`](../series/)‑samlingen i ett diagram. |
| [AddR1C1](../../aspose.cells.charts/seriescollection/addr1c1/)(string, bool) | Lägger till [`Series`](../series/)‑samlingen i ett diagram. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(Series) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(Series, IComparer&lt;Series&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, Series, IComparer&lt;Series&gt;) |  |
| [ChangeColors](../../aspose.cells.charts/seriescollection/changecolors/)(ChartColorPaletteType) | Ställ in monokromatisk palett för diagramserier. |
| [ChangeSeriesOrder](../../aspose.cells.charts/seriescollection/changeseriesorder/)(int, int) | (**Föråldrad.**) Ändrar direkt ordningen för de två serierna. |
| [Clear](../../aspose.cells.charts/seriescollection/clear/#clear)() | Rensar samlingen (2 metoder) |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(Series) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(Series[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(Series[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, Series[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;Series&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;Series&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;Series&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;Series&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;Series&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;Series&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;Series&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;Series&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;Series&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;Series&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [GetSeriesByOrder](../../aspose.cells.charts/seriescollection/getseriesbyorder/)(int) | Hämtar [`Series`](../series/)‑elementet efter ordning. |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Series) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Series, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Series, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Series) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Series, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Series, int, int) |  |
| [RemoveAt](../../aspose.cells.charts/seriescollection/removeat/#removeat)(int) | Tar bort en serie på det specifika indexet. (2 metoder) |
| [SetSeriesNames](../../aspose.cells.charts/seriescollection/setseriesnames/)(int, string, bool) | Anger namnen på alla serier i diagrammet. |
| [SwapSeries](../../aspose.cells.charts/seriescollection/swapseries/)(int, int) | Ändrar direkt ordningen för de två serierna. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class SeriesCollectionDemo
    {
        public static void SeriesCollectionExample()
        {
            // Instansiering av ett Workbook-objekt
            Workbook workbook = new Workbook();
            
            // Lägger till ett nytt kalkylblad i Excel-objektet
            int sheetIndex = workbook.Worksheets.Add();
            
            // Hämtar referensen till det nyligen tillagda kalkylbladet genom att ange dess bladindex
            Worksheet worksheet = workbook.Worksheets[sheetIndex];
            
            // Lägger till exempelvärden i celler
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["A4"].PutValue(200);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);
            worksheet.Cells["B4"].PutValue(40);
            worksheet.Cells["C1"].PutValue("Q1");
            worksheet.Cells["C2"].PutValue("Q2");
            worksheet.Cells["C3"].PutValue("Y1");
            worksheet.Cells["C4"].PutValue("Y2");

            // Lägger till ett diagram i kalkylbladet
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            
            // Åtkomst till instansen av det nyligen tillagda diagrammet
            Chart chart = worksheet.Charts[chartIndex];
            
            // Lägger till NSeries (diagramdatakälla) i diagrammet från cellen "A1" till "B4"
            chart.NSeries.Add("A1:B4", true);
            
            // Anger datakällan för kategoridata i NSeries
            chart.NSeries.CategoryData = "C1:C4";

            // Åtkomst till SeriesCollection i diagrammet
            SeriesCollection seriesCollection = chart.NSeries;

            // Anger egenskaper för SeriesCollection
            seriesCollection.CategoryData = "C1:C4";
            seriesCollection.SecondCategoryData = "C1:C4";
            seriesCollection.IsColorVaried = true;

            // Åtkomst till en specifik serie i SeriesCollection
            Series series = seriesCollection[0];
            
            // Anger egenskaper för serien
            series.Values = "=B1:B4";
            series.Name = "First Series";
            series.Type = ChartType.Line;
            series.Marker.MarkerStyle = ChartMarkerType.Circle;
            series.Marker.ForegroundColorSetType = FormattingType.Automatic;
            series.Marker.ForegroundColor = System.Drawing.Color.Black;
            series.Marker.BackgroundColorSetType = FormattingType.Automatic;

            // Sparar Excel-filen
            workbook.Save("SeriesCollectionExample.xlsx");
        }
    }
}
```

### Se även

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [Series](../series/)
* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


