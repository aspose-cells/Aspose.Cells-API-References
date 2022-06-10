---
title: TrendlineCollection
second_title: Aspose.Cells for .NET API Reference
description: Represents a collection of all the Trendline./trendline objects for the specified data series.
type: docs
weight: 1000
url: /net/aspose.cells.charts/trendlinecollection/
---
## TrendlineCollection class

Represents a collection of all the [`Trendline`](../trendline) objects for the specified data series.

```csharp
public class TrendlineCollection : CollectionBase<Trendline>
```

## Properties

| Name | Description |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase`1/capacity) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase`1/count) { get; } |  |
| [Item](../../aspose.cells.charts/trendlinecollection/item) { get; } | Gets a  object by its index. |
| [Item](../../aspose.cells/collectionbase`1/item) { get; set; } |  |

## Methods

| Name | Description |
| --- | --- |
| [Add](../../aspose.cells.charts/trendlinecollection/add#add)(TrendlineType) | Adds a  object to this collection with specified type. |
| [Add](../../aspose.cells.charts/trendlinecollection/add#add_1)(TrendlineType, string) | Adds a  object to this collection with specified type and name. |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(Trendline) |  |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(Trendline, IComparer&lt;Trendline&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(int, int, Trendline, IComparer&lt;Trendline&gt;) |  |
| [Clear](../../aspose.cells/collectionbase`1/clear)() |  |
| [Contains](../../aspose.cells/collectionbase`1/contains)(Trendline) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(Trendline[]) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(Trendline[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(int, Trendline[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase`1/exists)(Predicate&lt;Trendline&gt;) |  |
| [Find](../../aspose.cells/collectionbase`1/find)(Predicate&lt;Trendline&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase`1/findall)(Predicate&lt;Trendline&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(Predicate&lt;Trendline&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(int, Predicate&lt;Trendline&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(int, int, Predicate&lt;Trendline&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase`1/findlast)(Predicate&lt;Trendline&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(Predicate&lt;Trendline&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(int, Predicate&lt;Trendline&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(int, int, Predicate&lt;Trendline&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase`1/getenumerator)() |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(Trendline) |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(Trendline, int) |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(Trendline, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(Trendline) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(Trendline, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(Trendline, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase`1/removeat)(int) |  |

### Examples

```csharp
[C#]

//Instantiating a Workbook object
Workbook workbook = new Workbook();
//Adding a new worksheet to the Excel object
int sheetIndex = workbook.Worksheets.Add();
//Obtaining the reference of the newly added worksheet by passing its sheet index
Worksheet worksheet = workbook.Worksheets[sheetIndex];
worksheet.Cells["A1"].PutValue(50);
worksheet.Cells["A2"].PutValue(100);
worksheet.Cells["A3"].PutValue(150);
worksheet.Cells["A4"].PutValue(200);
worksheet.Cells["B1"].PutValue(60);
worksheet.Cells["B2"].PutValue(32);
worksheet.Cells["B3"].PutValue(50);
worksheet.Cells["B4"].PutValue(40);

//Adding a chart to the worksheet
int chartIndex = workbook.Worksheets[0].Charts.Add(ChartType.Column, 3, 3, 15, 10);
Chart chart = workbook.Worksheets[0].Charts[chartIndex];
chart.NSeries.Add("A1:a3", true);
chart.NSeries[0].TrendLines.Add(TrendlineType.Linear, "MyTrendLine");
Trendline line = chart.NSeries[0].TrendLines[0];
line.DisplayEquation = true;
line.DisplayRSquared = true;
line.Color = Color.Red;

[Visual Basic]

'Instantiating a Workbook object
Dim workbook As Workbook = New Workbook()
'Adding a new worksheet to the Excel object
Dim sheetIndex As Int32 = workbook.Worksheets.Add()
'Obtaining the reference of the newly added worksheet by passing its sheet index
Dim worksheet As Worksheet = workbook.Worksheets(sheetIndex)
worksheet.Cells("A1").PutValue(50)
worksheet.Cells("A2").PutValue(100)
worksheet.Cells("A3").PutValue(150)
worksheet.Cells("A4").PutValue(200)
worksheet.Cells("B1").PutValue(60)
worksheet.Cells("B2").PutValue(32)
worksheet.Cells("B3").PutValue(50)
worksheet.Cells("B4").PutValue(40)

'Adding a chart to the worksheet
Dim chartIndex As Integer =  workbook.Worksheets(0).Charts.Add(ChartType.Column,3,3,15,10) 
Dim chart As Chart =  workbook.Worksheets(0).Charts(chartIndex) 
chart.NSeries.Add("A1:a3", True)
chart.NSeries(0).TrendLines.Add(TrendlineType.Linear, "MyTrendLine")
Dim line As Trendline =  chart.NSeries(0).TrendLines(0) 
line.DisplayEquation = True
line.DisplayRSquared = True
line.Color = Color.Red
```

### See Also

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1)
* class [Trendline](../trendline)
* namespace [Aspose.Cells.Charts](../../aspose.cells.charts)
* assembly [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
