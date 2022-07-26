---
title: SeriesCollection
second_title: Aspose.Cells für .NET-API-Referenz
description: Kapselt eine Sammlung vonSeries./series Objekte.
type: docs
weight: 830
url: /de/net/aspose.cells.charts/seriescollection/
---
## SeriesCollection class

Kapselt eine Sammlung von[`Series`](../series) Objekte.

```csharp
public class SeriesCollection : CollectionBase<Series>
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase`1/capacity) { get; set; } |  |
| [CategoryData](../../aspose.cells.charts/seriescollection/categorydata) { get; set; } | Ruft den Bereich der Kategorieachsenwerte ab oder legt ihn fest. Dies kann eine Reihe von Zellen sein (z. B. „d1:e10“), oder eine Folge von Werten (z. B. „{2,6,8,10}“). |
| [Count](../../aspose.cells/collectionbase`1/count) { get; } |  |
| [IsColorVaried](../../aspose.cells.charts/seriescollection/iscolorvaried) { get; set; } | Stellt dar, ob die Farbe der Punkte variiert wird. |
| [Item](../../aspose.cells.charts/seriescollection/item) { get; } | Ruft die ab[`Series`](../series) Element am angegebenen Index. |
| [Item](../../aspose.cells/collectionbase`1/item) { get; set; } |  |
| [SecondCategoryData](../../aspose.cells.charts/seriescollection/secondcategorydata) { get; set; } | Ruft den Bereich der Achsenwerte der zweiten Kategorie ab oder legt ihn fest. Dies kann eine Reihe von Zellen sein (z. B. „d1:e10“), oder eine Folge von Werten (z. B. „{2,6,8,10}“). Wirkt sich nur aus, wenn einige ASeries auf der zweiten Achse dargestellt werden. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [Add](../../aspose.cells.charts/seriescollection/add#add)(string, bool) | Fügt die hinzu[`SeriesCollection`](../seriescollection) Sammlung zu einem Diagramm. |
| [Add](../../aspose.cells.charts/seriescollection/add#add_1)(string, bool, bool) | Fügt die hinzu[`SeriesCollection`](../seriescollection) Sammlung zu einem Diagramm. |
| [AddR1C1](../../aspose.cells.charts/seriescollection/addr1c1)(string, bool) | Fügt die hinzu[`SeriesCollection`](../seriescollection) Sammlung zu einem Diagramm. |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(Series) |  |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(Series, IComparer&lt;Series&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(int, int, Series, IComparer&lt;Series&gt;) |  |
| [ChangeSeriesOrder](../../aspose.cells.charts/seriescollection/changeseriesorder)(int, int) | Ändert direkt die Reihenfolge der beiden Serien. |
| [Clear](../../aspose.cells.charts/seriescollection/clear#clear)() | Löscht die Sammlung (2 methods) |
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
| [GetSeriesByOrder](../../aspose.cells.charts/seriescollection/getseriesbyorder)(int) | Ruft die ab[`Series`](../series) Element nach Bestellung. |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(Series) |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(Series, int) |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(Series, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(Series) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(Series, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(Series, int, int) |  |
| [RemoveAt](../../aspose.cells.charts/seriescollection/removeat#removeat)(int) | Entfernen Sie bei einer Reihe am spezifischen Index. (2 methods) |
| [SetSeriesNames](../../aspose.cells.charts/seriescollection/setseriesnames)(int, string, bool) | Legt den Namen aller Serien im Diagramm fest. |

### Beispiele

```csharp

[C#]
//Instanziieren eines Workbook-Objekts
Workbook workbook = new Workbook();
//Hinzufügen eines neuen Arbeitsblatts zum Excel-Objekt
int sheetIndex = workbook.Worksheets.Add();
//Beziehen der Referenz des neu hinzugefügten Arbeitsblatts durch Übergeben seines Blattindex
Worksheet worksheet = workbook.Worksheets[sheetIndex];
//Hinzufügen eines Beispielwerts zur Zelle "A1".
worksheet.Cells["A1"].PutValue(50);
//Hinzufügen eines Beispielwerts zur Zelle "A2".
worksheet.Cells["A2"].PutValue(100);
//Hinzufügen eines Beispielwerts zur Zelle "A3".
worksheet.Cells["A3"].PutValue(150);
//Hinzufügen eines Beispielwerts zur Zelle "A4".
worksheet.Cells["A4"].PutValue(200);
//Hinzufügen eines Beispielwerts zur Zelle "B1".
worksheet.Cells["B1"].PutValue(60);
//Hinzufügen eines Beispielwerts zur Zelle "B2".
worksheet.Cells["B2"].PutValue(32);
//Hinzufügen eines Beispielwerts zur Zelle "B3".
worksheet.Cells["B3"].PutValue(50);
//Hinzufügen eines Beispielwerts zur Zelle "B4".
worksheet.Cells["B4"].PutValue(40);
//Hinzufügen eines Beispielwerts zur Zelle "C1" als Kategoriedaten
worksheet.Cells["C1"].PutValue("Q1");
//Hinzufügen eines Beispielwerts zur Zelle "C2" als Kategoriedaten
worksheet.Cells["C2"].PutValue("Q2");
//Hinzufügen eines Beispielwerts zur Zelle "C3" als Kategoriedaten
worksheet.Cells["C3"].PutValue("Y1");
//Hinzufügen eines Beispielwerts zur Zelle "C4" als Kategoriedaten
worksheet.Cells["C4"].PutValue("Y2");
//Hinzufügen eines Diagramms zum Arbeitsblatt
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
//Auf die Instanz des neu hinzugefügten Diagramms zugreifen
Chart chart = worksheet.Charts[chartIndex];
//Hinzufügen von NSeries (Diagrammdatenquelle) zum Diagramm im Bereich von Zelle "A1" bis "B4"
chart.NSeries.Add("A1:B4", true);
//Festlegen der Datenquelle für die Kategoriedaten von NSeries
chart.NSeries.CategoryData = "C1:C4";
//Speichern der Excel-Datei
workbook.Save("book1.xls");

[Visual Basic]

'Instanziieren eines Workbook-Objekts
Dim workbook As Workbook = New Workbook()
'Hinzufügen eines neuen Arbeitsblatts zum Excel-Objekt
Dim sheetIndex As Integer = workbook.Worksheets.Add()
'Abrufen der Referenz des neu hinzugefügten Arbeitsblatts durch Übergeben seines Blattindex
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
'Hinzufügen eines Diagramms zum Arbeitsblatt
Dim chartIndex As Integer = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5)
'Zugriff auf die Instanz des neu hinzugefügten Diagramms
Dim chart As Chart = worksheet.Charts(chartIndex)
'Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B4"
chart.NSeries.Add("A1:B4", True)
'Festlegen der Datenquelle für die Kategoriedaten von NSeries
chart.NSeries.CategoryData = "C1:C4"
'Speichern der Excel-Datei
workbook.Save("book1.xls")
```

### Siehe auch

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1)
* class [Series](../series)
* namensraum [Aspose.Cells.Charts](../../aspose.cells.charts)
* Montage [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
