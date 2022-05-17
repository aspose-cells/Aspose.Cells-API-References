---
title: ChartPoint
second_title: Aspose.Cells for .NET API Reference
description: 
type: docs
weight: 500
url: /net/aspose.cells.charts/chartpoint/
---
## ChartPoint class

Represents a single point in a series in a chart.

```csharp
public class ChartPoint
```

## Properties

| Name | Description |
| --- | --- |
| [ArcEndPointXPx](arcendpointxpx) { get; } | Gets the x coordinate of ending point for the pie section after calls Chart.Calculate() method. Applies to Pie and Doughnut chart. |
| [ArcEndPointYPx](arcendpointypx) { get; } | Gets the y coordinate of ending point for the pie section after calls Chart.Calculate() method. Applies to Pie and Doughnut chart. |
| [ArcStartPointXPx](arcstartpointxpx) { get; } | Gets the x coordinate of starting point for the pie section after calls Chart.Calculate() method. Applies to Pie and Doughnut chart. |
| [ArcStartPointYPx](arcstartpointypx) { get; } | Gets the y coordinate of starting point for the pie section after calls Chart.Calculate() method. Applies to Pie and Doughnut chart. |
| [Area](area) { get; } | Gets the [`area`](./area). |
| [Border](border) { get; } | Gets the [`border`](../../aspose.cells.drawing/line). |
| [BorderWidthPx](borderwidthpx) { get; } | Gets the width of border in units of pixels after calls Chart.Calculate() method. |
| [DataLabels](datalabels) { get; } | Returns a DataLabels object that represents the data label associated with the point. |
| [EndAngle](endangle) { get; } | Gets the ending angle for the pie section, measured in degrees clockwise from the x-axis after calls Chart.Calculate() method. Applies to Pie chart. |
| [Explosion](explosion) { get; set; } | The distance of an open pie slice from the center of the pie chart is expressed as a percentage of the pie diameter. |
| [InnerArcEndPointXPx](innerarcendpointxpx) { get; } | Gets the x coordinate of ending point for the pie section after calls Chart.Calculate() method. Applies to Doughnut chart. |
| [InnerArcEndPointYPx](innerarcendpointypx) { get; } | Gets the y coordinate of ending point for the pie section after calls Chart.Calculate() method. Applies to Doughnut chart. |
| [InnerArcStartPointXPx](innerarcstartpointxpx) { get; } | Gets the x coordinate of starting point for the pie section after calls Chart.Calculate() method. Applies to Doughnut chart. |
| [InnerArcStartPointYPx](innerarcstartpointypx) { get; } | Gets the y coordinate of starting point for the pie section after calls Chart.Calculate() method. Applies to Doughnut chart. |
| [InnerRadiusPx](innerradiuspx) { get; } | Gets the inner radius of doughnut slice in units of pixels after calls Chart.Calculate() method. Applies to Doughnut chart. |
| [IsInSecondaryPlot](isinsecondaryplot) { get; set; } | Gets or sets a value indicates whether this data points is in the second pie or bar on a pie of pie or bar of pie chart |
| [Marker](marker) { get; } | Gets the [`marker`](./marker). |
| [RadiusPx](radiuspx) { get; } | Gets the radius of bubble, pie or doughnut in units of pixels after calls Chart.Calculate() method. |
| [Shadow](shadow) { get; set; } | True if the chartpoint has a shadow. |
| [ShapeHeight](shapeheight) { get; } | Gets the height in units of 1/4000 of chart's height after calls Chart.Calculate() method. |
| [ShapeHeightPx](shapeheightpx) { get; } | Gets the height in units of pixels after calls Chart.Calculate() method. |
| [ShapeProperties](shapeproperties) { get; } | Gets the  object that holds the visual shape properties of the ChartPoint. |
| [ShapeWidth](shapewidth) { get; } | Gets the width in units of 1/4000 of chart's width after calls Chart.Calculate() method. |
| [ShapeWidthPx](shapewidthpx) { get; } | Gets the width in units of pixels after calls Chart.Calculate() method. |
| [ShapeX](shapex) { get; } | Gets the x coordinate of the upper left corner in units of 1/4000 of chart's width after calls Chart.Calculate() method. |
| [ShapeXPx](shapexpx) { get; } | Gets the x coordinate of the upper left corner in units of pixels after calls Chart.Calculate() method. |
| [ShapeY](shapey) { get; } | Gets the y coordinate of the upper left corner in units of 1/4000 of chart's height after calls Chart.Calculate() method. |
| [ShapeYPx](shapeypx) { get; } | Gets the y coordinate of the upper left corner in units of pixels after calls Chart.Calculate() method. |
| [StartAngle](startangle) { get; } | Gets the starting angle for the pie section, measured in degrees clockwise from the x-axis after calls Chart.Calculate() method. Applies to Pie chart. |
| [XValue](xvalue) { get; set; } | Gets or sets the X value of the chart point. |
| [XValueType](xvaluetype) { get; } | Gets X value type of the chart point. |
| [YValue](yvalue) { get; set; } | Gets or sets the Y value of the chart point. |
| [YValueType](yvaluetype) { get; } | Gets Y value type of the chart point. |

## Methods

| Name | Description |
| --- | --- |
| [GetBottomPointCount](getbottompointcount)() | Gets the number of bottom points after calls Chart.Calculate() method. |
| [GetBottomPointXPx](getbottompointxpx)(int) | Gets x-coordinate of the bottom point of shape after calls Chart.Calculate() method. Applies 3D charts: Column3D, Bar3D, Cone, Cylinder, Pyramid |
| [GetBottomPointYPx](getbottompointypx)(int) | Gets y-coordinate of the bottom point of shape after calls Chart.Calculate() method. Applies 3D charts: Column3D, Bar3D, Cone, Cylinder, Pyramid |
| [GetOnCategoryAxisPointCount](getoncategoryaxispointcount)() | Gets the number of the points on category axis after calls Chart.Calculate() method. Only applies to area chart. |
| [GetOnCategoryAxisPointXPx](getoncategoryaxispointxpx)(int) | Gets x-coordinate of the point on category axis after calls Chart.Calculate() method. Only applies to Area chart. |
| [GetOnCategoryAxisPointYPx](getoncategoryaxispointypx)(int) | Gets y-coordinate of the point on category axis after calls Chart.Calculate() method. Only applies to Area chart. |
| [GetTopPointCount](gettoppointcount)() | Gets the number of top points after calls Chart.Calculate() method. |
| [GetTopPointXPx](gettoppointxpx)(int) | Gets x-coordinate of the top point of shape after calls Chart.Calculate() method. Applies 3D charts: Column3D, Bar3D, Cone, Cylinder, Pyramid and Area3D |
| [GetTopPointYPx](gettoppointypx)(int) | Gets y-coordinate of the top point of shape after calls Chart.Calculate() method. Applies 3D charts: Column3D, Bar3D, Cone, Cylinder, Pyramid and Area3D |

### Examples

```csharp

[C#]

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
chart.NSeries[0].DataLabels.IsValueShown = true;

for (int i = 0; i  < chart.NSeries[0].Points.Count; i++)
{
    //Get Data Point
    ChartPoint point = chart.NSeries[0].Points[i];
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
chart.NSeries(0).DataLabels.IsValueShown = True

For i As Integer = 0 To chart.NSeries(0).Points.Count - 1
    'Get Data Point
    Dim point As ChartPoint = chart.NSeries(0).Points(i)
    'Set Pir Explosion
    point.Explosion = 15
    'Set Border Color
    point.Border.Color = System.Drawing.Color.Red
Next i

'Saving the Excel file
workbook.Save("book1.xls")

```

### See Also

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts)
* assembly [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
