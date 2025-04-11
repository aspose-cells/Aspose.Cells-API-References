---
title: Class ChartPointCollection
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Charts.ChartPointCollection class. Represents a collection that contains all the points in one series
type: docs
url: /net/aspose.cells.charts/chartpointcollection/
---
## ChartPointCollection class

Represents a collection that contains all the points in one series.

```csharp
public class ChartPointCollection : IEnumerable
```

## Properties

| Name | Description |
| --- | --- |
| [Count](../../aspose.cells.charts/chartpointcollection/count/) { get; } | Gets the count of the chart point. |
| [Item](../../aspose.cells.charts/chartpointcollection/item/) { get; } | Gets the [`ChartPoint`](../chartpoint/) element at the specified index in the series. |

## Methods

| Name | Description |
| --- | --- |
| [Clear](../../aspose.cells.charts/chartpointcollection/clear/)() | Remove all setting of the chart points. |
| [GetEnumerator](../../aspose.cells.charts/chartpointcollection/getenumerator/)() | Returns an enumerator for the entire `ChartPointCollection`. |
| [RemoveAt](../../aspose.cells.charts/chartpointcollection/removeat/)(int) | Removes point at the index of the series.. |

### Examples

```csharp
//Instantiating a Workbook object
Workbook workbook = new Workbook();

//Obtaining the reference of the first worksheet
Worksheet worksheet = workbook.Worksheets[0];

//Adding a sample value to "A1" cell
worksheet.Cells["A1"].PutValue(50);

//Adding a sample value to "A2" cell
worksheet.Cells["A2"].PutValue(100);

//Adding a sample value to "A3" cell
worksheet.Cells["A3"].PutValue(150);

//Adding a sample value to "B1" cell
worksheet.Cells["B1"].PutValue(60);

//Adding a sample value to "B2" cell
worksheet.Cells["B2"].PutValue(32);

//Adding a sample value to "B3" cell
worksheet.Cells["B3"].PutValue(50);

//Adding a chart to the worksheet
int chartIndex = worksheet.Charts.Add(ChartType.PieExploded, 5, 0, 25, 10);

//Accessing the instance of the newly added chart
Chart chart = worksheet.Charts[chartIndex];

//Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B3"
chart.NSeries.Add("A1:B3", true);

//Show Data Labels 
chart.NSeries[0].DataLabels.ShowValue = true;

ChartPointCollection points = chart.NSeries[0].Points;

for (int i = 0; i < points.Count; i++)
{
    //Get Data Point
    ChartPoint point = points[i];
    //Set Pir Explosion
    point.Explosion = 15;
    //Set Border Color
    point.Border.Color = System.Drawing.Color.Red;
}

//Saving the Excel file
workbook.Save("book1.xls");

[VB.NET]

'Instantiating a Workbook object
Dim workbook As Workbook = New Workbook()

'Obtaining the reference of the first worksheet
Dim worksheet As Worksheet = workbook.Worksheets(0)

'Adding a sample value to "A1" cell
worksheet.Cells("A1").PutValue(50)

'Adding a sample value to "A2" cell
worksheet.Cells("A2").PutValue(100)

'Adding a sample value to "A3" cell
worksheet.Cells("A3").PutValue(150)

'Adding a sample value to "B1" cell
worksheet.Cells("B1").PutValue(60)

'Adding a sample value to "B2" cell
worksheet.Cells("B2").PutValue(32)

'Adding a sample value to "B3" cell
worksheet.Cells("B3").PutValue(50)

'Adding a chart to the worksheet
Dim chartIndex As Integer = worksheet.Charts.Add(ChartType.PieExploded, 5, 0, 25, 10)

'Accessing the instance of the newly added chart
Dim chart As Chart = worksheet.Charts(chartIndex)

'Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B3"
chart.NSeries.Add("A1:B3", True)

'Show Data Labels 
chart.NSeries(0).DataLabels.ShowValue = True

Dim points As ChartPointCollection = chart.NSeries(0).Points

For i As Integer = 0 To points.Count - 1
    'Get Data Point
    Dim point As ChartPoint = points(i)
    'Set Pir Explosion
    point.Explosion = 15
    'Set Border Color
    point.Border.Color = System.Drawing.Color.Red
Next i

'Saving the Excel file
workbook.Save("book1.xls")

```

### See Also

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


