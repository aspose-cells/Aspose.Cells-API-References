---
title: DataLabels.SeparatorValue
second_title: Aspose.Cells for .NET API Reference
description: DataLabels property. Gets or sets the separator value used for the data labels on a chart
type: docs
url: /net/aspose.cells.charts/datalabels/separatorvalue/
---
## DataLabels.SeparatorValue property

Gets or sets the separator value used for the data labels on a chart.

```csharp
public string SeparatorValue { get; set; }
```

### Examples

```csharp
// Called: dataLabels.SeparatorValue = ", ";
public static void DataLabels_Property_SeparatorValue()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();

            // Access the first worksheet
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Add a chart to the worksheet
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Add series to the chart
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Access the DataLabels of the first series
            DataLabels dataLabels = chart.NSeries[0].DataLabels;

            // Set properties of DataLabels
            dataLabels.Position = LabelPositionType.InsideBase;
            dataLabels.ShowCategoryName = true;
            dataLabels.ShowValue = true;
            dataLabels.ShowPercentage = false;
            dataLabels.ShowLegendKey = false;
            dataLabels.IsAutoText = true;
            dataLabels.DirectionType = ChartTextDirectionType.Horizontal;
            dataLabels.Text = "Custom Text";
            dataLabels.IsTextWrapped = true;
            dataLabels.BackgroundMode = BackgroundMode.Transparent;
            dataLabels.ShowCellRange = false;
            dataLabels.ShowBubbleSize = false;
            dataLabels.ShowSeriesName = false;
            dataLabels.NumberFormat = "0.00";
            dataLabels.Number = 0;
            dataLabels.NumberFormatLinked = false;
            dataLabels.SeparatorType = DataLabelsSeparatorType.Comma;
            dataLabels.SeparatorValue = ", ";
            dataLabels.IsNeverOverlap = true;
            dataLabels.IsDeleted = false;
            dataLabels.TextHorizontalAlignment = TextAlignmentType.Center;
            dataLabels.TextVerticalAlignment = TextAlignmentType.Center;
            dataLabels.RotationAngle = 0;
            dataLabels.LinkedSource = "";
            dataLabels.TextDirection = TextDirectionType.LeftToRight;
            dataLabels.ReadingOrder = TextDirectionType.LeftToRight;
            dataLabels.IsResizeShapeToFitText = true;
            dataLabels.IsInnerMode = false;
            dataLabels.AutoScaleFont = true;
            dataLabels.Background = BackgroundMode.Transparent;
            dataLabels.IsAutomaticSize = true;
            dataLabels.X = 0;
            dataLabels.Y = 0;
            dataLabels.Height = 100;
            dataLabels.Width = 100;
            dataLabels.Shadow = false;

            // Save the workbook
            workbook.Save("DataLabelsExample.xlsx");
            workbook.Save("DataLabelsExample.pdf");
        }
```

### See Also

* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


