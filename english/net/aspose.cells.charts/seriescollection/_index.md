---
title: SeriesCollection
second_title: Aspose.Cells for .NET API Reference
description: 
type: docs
weight: 820
url: /net/aspose.cells.charts/seriescollection/
---
## SeriesCollection class

Encapsulates a collection of [`Series`](../series) objects.

```csharp
public class SeriesCollection : CollectionBase<Series>
```

## Properties

| Name | Description |
| --- | --- |
| [CategoryData](categorydata) { get; set; } | Gets or sets the range of category Axis values. It can be a range of cells (such as, "d1:e10"), or a sequence of values (such as,"{2,6,8,10}"). |
| [IsColorVaried](iscolorvaried) { get; set; } | Represents if the color of points is varied. |
| [Item](item) { get; } | Gets the [`Series`](../series) element at the specified index. |
| [SecondCategoryData](secondcategorydata) { get; set; } | Gets or sets the range of second category Axis values. It can be a range of cells (such as, "d1:e10"), or a sequence of values (such as,"{2,6,8,10}"). Only effects when some ASerieses plot on the second axis. |

## Methods

| Name | Description |
| --- | --- |
| [Add](add)(string, bool) | Adds the [`SeriesCollection`](../seriescollection) collection to a chart. |
| [Add](add)(string, bool, bool) | Adds the [`SeriesCollection`](../seriescollection) collection to a chart. |
| [AddR1C1](addr1c1)(string, bool) | Adds the [`SeriesCollection`](../seriescollection) collection to a chart. |
| [ChangeSeriesOrder](changeseriesorder)(int, int) | Directly changes the orders of the two series. |
| [Clear](clear)() | Clears the collection |
| [GetSeriesByOrder](getseriesbyorder)(int) | Gets the [`Series`](../series) element by order. |
| [RemoveAt](removeat)(int) | Remove at a series at the specific index. |
| [SetSeriesNames](setseriesnames)(int, string, bool) | Sets the name of all the serieses in the chart. |

### Examples

```csharp

[C#]
//Instantiating a Workbook object
Workbook workbook = new Workbook();
//Adding a new worksheet to the Excel object
int sheetIndex = workbook.Worksheets.Add();
//Obtaining the reference of the newly added worksheet by passing its sheet index
Worksheet worksheet = workbook.Worksheets[sheetIndex];
//Adding a sample value to "A1" cell
worksheet.Cells["A1"].PutValue(50);
//Adding a sample value to "A2" cell
worksheet.Cells["A2"].PutValue(100);
//Adding a sample value to "A3" cell
worksheet.Cells["A3"].PutValue(150);
//Adding a sample value to "A4" cell
worksheet.Cells["A4"].PutValue(200);
//Adding a sample value to "B1" cell
worksheet.Cells["B1"].PutValue(60);
//Adding a sample value to "B2" cell
worksheet.Cells["B2"].PutValue(32);
//Adding a sample value to "B3" cell
worksheet.Cells["B3"].PutValue(50);
//Adding a sample value to "B4" cell
worksheet.Cells["B4"].PutValue(40);
//Adding a sample value to "C1" cell as category data
worksheet.Cells["C1"].PutValue("Q1");
//Adding a sample value to "C2" cell as category data
worksheet.Cells["C2"].PutValue("Q2");
//Adding a sample value to "C3" cell as category data
worksheet.Cells["C3"].PutValue("Y1");
//Adding a sample value to "C4" cell as category data
worksheet.Cells["C4"].PutValue("Y2");
//Adding a chart to the worksheet
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
//Accessing the instance of the newly added chart
Chart chart = worksheet.Charts[chartIndex];
//Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B4"
chart.NSeries.Add("A1:B4", true);
//Setting the data source for the category data of NSeries
chart.NSeries.CategoryData = "C1:C4";
//Saving the Excel file
workbook.Save("book1.xls");

[Visual Basic]

'Instantiating a Workbook object
Dim workbook As Workbook = New Workbook()
'Adding a new worksheet to the Excel object
Dim sheetIndex As Integer = workbook.Worksheets.Add()
'Obtaining the reference of the newly added worksheet by passing its sheet index
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
'Adding a chart to the worksheet
Dim chartIndex As Integer = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5)
'Accessing the instance of the newly added chart
Dim chart As Chart = worksheet.Charts(chartIndex)
'Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B4"
chart.NSeries.Add("A1:B4", True)
'Setting the data source for the category data of NSeries
chart.NSeries.CategoryData = "C1:C4"
'Saving the Excel file
workbook.Save("book1.xls")
```

### See Also

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1)
* class [Series](../series)
* namespace [Aspose.Cells.Charts](../../aspose.cells.charts)
* assembly [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
