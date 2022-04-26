---
title: SparklineGroup
second_title: Aspose.Cells for .NET API Reference
description: 
type: docs
weight: 870
url: /net/aspose.cells.charts/sparklinegroup/
---
## SparklineGroup class

[`Sparkline`](../sparkline) is organized into sparkline group. A SparklineGroup contains a variable number of sparkline items. A sparkline group specifies the type, display settings and axis settings for the sparklines.

```csharp
public class SparklineGroup
```

## Properties

| Name | Description |
| --- | --- |
| [DisplayHidden](displayhidden) { get; set; } | Indicates whether to show data in hidden rows and columns. |
| [FirstPointColor](firstpointcolor) { get; set; } | Gets and sets the color of the first point of data in the sparkline group. |
| [HighPointColor](highpointcolor) { get; set; } | Gets and sets the color of the highest points of data in the sparkline group. |
| [HorizontalAxisColor](horizontalaxiscolor) { get; set; } | Gets and sets the color of the horizontal axis in the sparkline group. |
| [HorizontalAxisDateRange](horizontalaxisdaterange) { get; set; } | Represents the range that contains the date values for the sparkline data. |
| [LastPointColor](lastpointcolor) { get; set; } | Gets and sets the color of the last point of data in the sparkline group. |
| [LineWeight](lineweight) { get; set; } | Gets and sets the line weight in each line sparkline in the sparkline group, in the unit of points. |
| [LowPointColor](lowpointcolor) { get; set; } | Gets and sets the color of the lowest points of data in the sparkline group. |
| [MarkersColor](markerscolor) { get; set; } | Gets and sets the color of points in each line sparkline in the sparkline group. |
| [NegativePointsColor](negativepointscolor) { get; set; } | Gets and sets the color of the negative values on the sparkline group. |
| [PlotEmptyCellsType](plotemptycellstype) { get; set; } | Indicates how to plot empty cells. |
| [PlotRightToLeft](plotrighttoleft) { get; set; } | Indicates whether the plot data is right to left. |
| [PresetStyle](presetstyle) { get; set; } | Gets and sets the preset style type of the sparkline group. |
| [SeriesColor](seriescolor) { get; set; } | Gets and sets the color of the sparklines in the sparkline group. |
| [ShowFirstPoint](showfirstpoint) { get; set; } | Indicates whether to highlight the first point of data in the sparkline group. |
| [ShowHighPoint](showhighpoint) { get; set; } | Indicates whether to highlight the highest points of data in the sparkline group. |
| [ShowHorizontalAxis](showhorizontalaxis) { get; set; } | Indicates whether to show the sparkline horizontal axis. The horizontal axis appears if the sparkline has data that crosses the zero axis. |
| [ShowLastPoint](showlastpoint) { get; set; } | Indicates whether to highlight the last point of data in the sparkline group. |
| [ShowLowPoint](showlowpoint) { get; set; } | Indicates whether to highlight the lowest points of data in the sparkline group. |
| [ShowMarkers](showmarkers) { get; set; } | Indicates whether to highlight each point in each line sparkline in the sparkline group. |
| [ShowNegativePoints](shownegativepoints) { get; set; } | Indicates whether to highlight the negative values on the sparkline group with a different color or marker. |
| [SparklineCollection](sparklinecollection) { get; } | Gets the [`SparklineCollection`](./sparklinecollection) object of the sparkline group. |
| [Type](type) { get; set; } | Indicates the sparkline type of the sparkline group. |
| [VerticalAxisMaxValue](verticalaxismaxvalue) { get; set; } | Gets and sets the custom maximum value for the vertical axis. |
| [VerticalAxisMaxValueType](verticalaxismaxvaluetype) { get; set; } | Represents the vertical axis maximum value type. |
| [VerticalAxisMinValue](verticalaxisminvalue) { get; set; } | Gets and sets the custom minimum value for the vertical axis. |
| [VerticalAxisMinValueType](verticalaxisminvaluetype) { get; set; } | Represents the vertical axis minimum value type. |

## Methods

| Name | Description |
| --- | --- |
| [ResetRanges](resetranges)(string, bool, CellArea) | Resets the data range and location range of the sparkline group. This method will clear original sparkline items in the group and creates new sparkline items for the new ranges. |

### Examples

```csharp
[C#]
 Workbook book = new Workbook(); 
 Worksheet sheet = book.Worksheets[0];

 sheet.Cells["A1"].PutValue(5);
 sheet.Cells["B1"].PutValue(2);
 sheet.Cells["C1"].PutValue(1);
 sheet.Cells["D1"].PutValue(3);
 
 // Define the CellArea
 CellArea ca = new CellArea();
 ca.StartColumn = 4;
 ca.EndColumn = 4;
 ca.StartRow = 0;
 ca.EndRow = 0;
 int idx = sheet.SparklineGroupCollection.Add(Aspose.Cells.Charts.SparklineType.Line, "A1:D1", false, ca);
 SparklineGroup group = sheet.SparklineGroupCollection[idx];
 group.SparklineCollection.Add(sheet.Name + "!A1:D1", 0, 4);
 // Create CellsColor
 CellsColor clr = book.CreateCellsColor();
 clr.Color = Color.Orange;
 group.SeriesColor = clr;

 // set the high points are colored green and the low points are colored red
 group.ShowHighPoint = true;
 group.ShowLowPoint = true;
 group.HighPointColor.Color = Color.Green;
 group.LowPointColor.Color = Color.Red;
 // set line weight 
 group.LineWeight = 1.0;
 book.Save("output.xlsx", SaveFormat.Xlsx);
```

### See Also

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts)
* assembly [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
