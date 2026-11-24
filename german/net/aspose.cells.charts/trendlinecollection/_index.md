---
title: "Klasse TrendlineCollection"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Charts.TrendlineCollection Klasse. Stellt eine Sammlung aller Trendline‑Objekte für die angegebene Datenreihe dar."
type: docs
url: /de/net/aspose.cells.charts/trendlinecollection/
---
## TrendlineCollection class

Stellt eine Sammlung aller [`Trendline`](../trendline/)‑Objekte für die angegebene Datenreihe dar.

```csharp
public class TrendlineCollection : CollectionBase<Trendline>
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.charts/trendlinecollection/item/) { get; } | Ruft ein [`Trendline`](../trendline/)‑Objekt anhand seines Index ab. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [Add](../../aspose.cells.charts/trendlinecollection/add/#add)(TrendlineType) | Fügt dieser Sammlung ein [`Trendline`](../trendline/)‑Objekt mit dem angegebenen Typ hinzu. |
| [Add](../../aspose.cells.charts/trendlinecollection/add/#add_1)(TrendlineType, string) | Fügt dieser Sammlung ein [`Trendline`](../trendline/)‑Objekt mit angegebenem Typ und Namen hinzu. |
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

### Beispiele

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
            // Instanziieren eines Workbook-Objekts
            Workbook workbook = new Workbook();
            
            // Ein neues Arbeitsblatt zum Excel-Objekt hinzufügen
            int sheetIndex = workbook.Worksheets.Add();
            
            // Abrufen der Referenz des neu hinzugefügten Arbeitsblatts durch Übergabe seines Blattindexes
            Worksheet worksheet = workbook.Worksheets[sheetIndex];
            
            // Hinzufügen von Beispielwerten zu Zellen
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["A4"].PutValue(200);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);
            worksheet.Cells["B4"].PutValue(40);

            // Hinzufügen eines Diagramms zum Arbeitsblatt
            int chartIndex = workbook.Worksheets[0].Charts.Add(ChartType.Column, 3, 3, 15, 10);
            Chart chart = workbook.Worksheets[0].Charts[chartIndex];
            
            // Hinzufügen von NSeries (Diagrammdatenquelle) zum Diagramm vom Feld "A1" bis "B4"
            chart.NSeries.Add("A1:A4", true);
            chart.NSeries.Add("B1:B4", true);
            
            // Hinzufügen einer Trendlinie zur ersten Serie
            int trendlineIndex = chart.NSeries[0].TrendLines.Add(TrendlineType.Linear, "MyTrendLine");
            Trendline trendline = chart.NSeries[0].TrendLines[trendlineIndex];
            
            // Festlegen von Trendlinien‑Eigenschaften
            trendline.DisplayEquation = true;
            trendline.DisplayRSquared = true;
            trendline.Color = Color.Red;

            // Die Excel-Datei speichern
            workbook.Save("TrendlineCollectionExample.xlsx");
        }
    }
}
```

### Siehe auch

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [Trendline](../trendline/)
* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


