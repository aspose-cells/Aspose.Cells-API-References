---
title: "Klasse SeriesCollection"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Charts.SeriesCollection Klasse. Kapselt eine Sammlung von Series-Objekten."
type: docs
url: /de/net/aspose.cells.charts/seriescollection/
---
## SeriesCollection class

Kapselt eine Sammlung von [`Series`](../series/) Objekten.

```csharp
public class SeriesCollection : CollectionBase<Series>
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [CategoryData](../../aspose.cells.charts/seriescollection/categorydata/) { get; set; } | Liest oder setzt den Bereich der Kategorienachsenwerte. Es kann ein Zellbereich sein (z. B. "d1:e10") oder eine Wertefolge (z. B. "{2,6,8,10}"). |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [IsColorVaried](../../aspose.cells.charts/seriescollection/iscolorvaried/) { get; set; } | Stellt dar, ob die Farbe der Punkte variiert. |
| [Item](../../aspose.cells.charts/seriescollection/item/) { get; } | Ruft das [`Series`](../series/) Element am angegebenen Index ab. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |
| [SecondCategoryData](../../aspose.cells.charts/seriescollection/secondcategorydata/) { get; set; } | Liest oder setzt den Bereich der zweiten Kategorienachsenwerte. Es kann ein Zellbereich sein (z. B. "d1:e10") oder eine Wertefolge (z. B. "{2,6,8,10}"). Wirkt nur, wenn einige Serien auf der zweiten Achse dargestellt wurden. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [Add](../../aspose.cells.charts/seriescollection/add/#add)(string, bool) | Fügt die [`Series`](../series/) Sammlung zu einem Diagramm hinzu. |
| [Add](../../aspose.cells.charts/seriescollection/add/#add_1)(string, bool, bool) | Fügt die [`Series`](../series/) Sammlung zu einem Diagramm hinzu. |
| [AddR1C1](../../aspose.cells.charts/seriescollection/addr1c1/)(string, bool) | Fügt die [`Series`](../series/) Sammlung zu einem Diagramm hinzu. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(Series) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(Series, IComparer&lt;Series&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, Series, IComparer&lt;Series&gt;) |  |
| [ChangeColors](../../aspose.cells.charts/seriescollection/changecolors/)(ChartColorPaletteType) | Setze eine monochrome Palette für Diagrammserien. |
| [ChangeSeriesOrder](../../aspose.cells.charts/seriescollection/changeseriesorder/)(int, int) | (**Obsolete.**) Ändert direkt die Reihenfolge der beiden Serien. |
| [Clear](../../aspose.cells.charts/seriescollection/clear/#clear)() | Löscht die Sammlung (2 Methoden) |
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
| [GetSeriesByOrder](../../aspose.cells.charts/seriescollection/getseriesbyorder/)(int) | Ruft das [`Series`](../series/) Element nach Reihenfolge ab. |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Series) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Series, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Series, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Series) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Series, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Series, int, int) |  |
| [RemoveAt](../../aspose.cells.charts/seriescollection/removeat/#removeat)(int) | Entfernt eine Serie am spezifischen Index. (2 Methoden) |
| [SetSeriesNames](../../aspose.cells.charts/seriescollection/setseriesnames/)(int, string, bool) | Setzt die Namen aller Serien im Diagramm. |
| [SwapSeries](../../aspose.cells.charts/seriescollection/swapseries/)(int, int) | Ändert direkt die Reihenfolge der beiden Serien. |

### Beispiele

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
            worksheet.Cells["C1"].PutValue("Q1");
            worksheet.Cells["C2"].PutValue("Q2");
            worksheet.Cells["C3"].PutValue("Y1");
            worksheet.Cells["C4"].PutValue("Y2");

            // Hinzufügen eines Diagramms zum Arbeitsblatt
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            
            // Zugriff auf die Instanz des neu hinzugefügten Diagramms
            Chart chart = worksheet.Charts[chartIndex];
            
            // Hinzufügen von NSeries (Diagrammdatenquelle) zum Diagramm vom Feld "A1" bis "B4"
            chart.NSeries.Add("A1:B4", true);
            
            // Festlegen der Datenquelle für die Kategoriedaten von NSeries
            chart.NSeries.CategoryData = "C1:C4";

            // Zugriff auf die SeriesCollection des Diagramms
            SeriesCollection seriesCollection = chart.NSeries;

            // Festlegen von Eigenschaften der SeriesCollection
            seriesCollection.CategoryData = "C1:C4";
            seriesCollection.SecondCategoryData = "C1:C4";
            seriesCollection.IsColorVaried = true;

            // Zugriff auf eine bestimmte Serie in der SeriesCollection
            Series series = seriesCollection[0];
            
            // Festlegen von Eigenschaften der Serie
            series.Values = "=B1:B4";
            series.Name = "First Series";
            series.Type = ChartType.Line;
            series.Marker.MarkerStyle = ChartMarkerType.Circle;
            series.Marker.ForegroundColorSetType = FormattingType.Automatic;
            series.Marker.ForegroundColor = System.Drawing.Color.Black;
            series.Marker.BackgroundColorSetType = FormattingType.Automatic;

            // Die Excel-Datei speichern
            workbook.Save("SeriesCollectionExample.xlsx");
        }
    }
}
```

### Siehe auch

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [Series](../series/)
* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


