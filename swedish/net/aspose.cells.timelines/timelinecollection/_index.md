---
title: TimelineCollection
second_title: Aspose.Cells för .NET API-referens
description: Anger samlingen av alla tidslinjeobjekt på det angivna kalkylbladet.
type: docs
weight: 6080
url: /sv/net/aspose.cells.timelines/timelinecollection/
---
## TimelineCollection class

Anger samlingen av alla tidslinjeobjekt på det angivna kalkylbladet.

```csharp
public class TimelineCollection : CollectionBase<Timeline>
```

## Egenskaper

| namn | Beskrivning |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase`1/capacity) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase`1/count) { get; } |  |
| [Item](../../aspose.cells.timelines/timelinecollection/item) { get; } | Hämtar tidslinjen efter index. (2 indexers) |
| [Item](../../aspose.cells/collectionbase`1/item) { get; set; } |  |

## Metoder

| namn | Beskrivning |
| --- | --- |
| [Add](../../aspose.cells.timelines/timelinecollection/add#add_4)(PivotTable, string, int) | Lägg till en ny tidslinje med pivottabell som datakälla |
| [Add](../../aspose.cells.timelines/timelinecollection/add#add_3)(PivotTable, string, PivotField) | Lägg till en ny tidslinje med pivottabell som datakälla |
| [Add](../../aspose.cells.timelines/timelinecollection/add#add_5)(PivotTable, string, string) | Lägg till en ny tidslinje med pivottabell som datakälla |
| [Add](../../aspose.cells.timelines/timelinecollection/add#add_1)(PivotTable, int, int, int) | Lägg till en ny tidslinje med pivottabell som datakälla |
| [Add](../../aspose.cells.timelines/timelinecollection/add#add)(PivotTable, int, int, PivotField) | Lägg till en ny tidslinje med pivottabell som datakälla |
| [Add](../../aspose.cells.timelines/timelinecollection/add#add_2)(PivotTable, int, int, string) | Lägg till en ny tidslinje med pivottabell som datakälla |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(Timeline) |  |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(Timeline, IComparer&lt;Timeline&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(int, int, Timeline, IComparer&lt;Timeline&gt;) |  |
| [Clear](../../aspose.cells/collectionbase`1/clear)() |  |
| [Contains](../../aspose.cells/collectionbase`1/contains)(Timeline) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(Timeline[]) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(Timeline[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(int, Timeline[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase`1/exists)(Predicate&lt;Timeline&gt;) |  |
| [Find](../../aspose.cells/collectionbase`1/find)(Predicate&lt;Timeline&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase`1/findall)(Predicate&lt;Timeline&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(Predicate&lt;Timeline&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(int, Predicate&lt;Timeline&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(int, int, Predicate&lt;Timeline&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase`1/findlast)(Predicate&lt;Timeline&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(Predicate&lt;Timeline&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(int, Predicate&lt;Timeline&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(int, int, Predicate&lt;Timeline&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase`1/getenumerator)() |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(Timeline) |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(Timeline, int) |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(Timeline, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(Timeline) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(Timeline, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(Timeline, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase`1/removeat)(int) |  |

### Exempel

```csharp

[C#]
Workbook book = new Workbook();
Worksheet sheet = book.Worksheets[0];
Cells cells = sheet.Cells;
cells[0, 0].Value = "fruit";
cells[1, 0].Value = "grape";
cells[2, 0].Value = "blueberry";
cells[3, 0].Value = "kiwi";
cells[4, 0].Value = "cherry";

//Skapa datumstil
Style dateStyle = new CellsFactory().CreateStyle();
dateStyle.Custom = "m/d/yyyy";
cells[0, 1].Value = "date";
cells[1, 1].Value = new DateTime(2021, 2, 5);
cells[2, 1].Value = new DateTime(2022, 3, 8);
cells[3, 1].Value = new DateTime(2023, 4, 10);
cells[4, 1].Value = new DateTime(2024, 5, 16);
//Ange datumstil
cells[1, 1].SetStyle(dateStyle);
cells[2, 1].SetStyle(dateStyle);
cells[3, 1].SetStyle(dateStyle);
cells[4, 1].SetStyle(dateStyle);

cells[0, 2].Value = "amount";
cells[1, 2].Value = 50;
cells[2, 2].Value = 60;
cells[3, 2].Value = 70;
cells[4, 2].Value = 80;

PivotTableCollection pivots = sheet.PivotTables;
//Lägg till en pivottabell
int pivotIndex = pivots.Add("=Sheet1!A1:C5", "A12", "TestPivotTable");
PivotTable pivot = pivots[pivotIndex];
pivot.AddFieldToArea(PivotFieldType.Row, "fruit");
pivot.AddFieldToArea(PivotFieldType.Column, "date");
pivot.AddFieldToArea(PivotFieldType.Data, "amount");
pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;

//Uppdatera pivottabelldata
pivot.RefreshData();
pivot.CalculateData();

//gör dina affärer
book.Save("out.xlsx");

```

### Se även

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1)
* class [Timeline](../timeline)
* namnutrymme [Aspose.Cells.Timelines](../../aspose.cells.timelines)
* hopsättning [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
