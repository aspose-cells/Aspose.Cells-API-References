---
title: Marker.ForegroundColorSetType
second_title: Aspose.Cells for .NET API Reference
description: Marker property. Gets or sets the marker foreground color set type
type: docs
url: /net/aspose.cells.charts/marker/foregroundcolorsettype/
---
## Marker.ForegroundColorSetType property

Gets or sets the marker foreground color set type.

```csharp
public FormattingType ForegroundColorSetType { get; set; }
```

### Examples

```csharp
// Called: series.Marker.ForegroundColorSetType = FormattingType.Automatic;
public static void Marker_Property_ForegroundColorSetType()
        {
            // Instantiating a Workbook object
            Workbook workbook = new Workbook();
            
            // Adding a new worksheet to the Excel object
            int sheetIndex = workbook.Worksheets.Add();
            
            // Obtaining the reference of the newly added worksheet by passing its sheet index
            Worksheet worksheet = workbook.Worksheets[sheetIndex];
            
            // Adding sample values to cells
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

            // Adding a chart to the worksheet
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            
            // Accessing the instance of the newly added chart
            Chart chart = worksheet.Charts[chartIndex];
            
            // Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B4"
            chart.NSeries.Add("A1:B4", true);
            
            // Setting the data source for the category data of NSeries
            chart.NSeries.CategoryData = "C1:C4";

            // Accessing the SeriesCollection of the chart
            SeriesCollection seriesCollection = chart.NSeries;

            // Setting properties of the SeriesCollection
            seriesCollection.CategoryData = "C1:C4";
            seriesCollection.SecondCategoryData = "C1:C4";
            seriesCollection.IsColorVaried = true;

            // Accessing a specific series in the SeriesCollection
            Series series = seriesCollection[0];
            
            // Setting properties of the series
            series.Values = "=B1:B4";
            series.Name = "First Series";
            series.Type = ChartType.Line;
            series.Marker.MarkerStyle = ChartMarkerType.Circle;
            series.Marker.ForegroundColorSetType = FormattingType.Automatic;
            series.Marker.ForegroundColor = System.Drawing.Color.Black;
            series.Marker.BackgroundColorSetType = FormattingType.Automatic;

            // Saving the Excel file
            workbook.Save("SeriesCollectionExample.xlsx");
        }
```

### See Also

* enum [FormattingType](../../formattingtype/)
* class [Marker](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


