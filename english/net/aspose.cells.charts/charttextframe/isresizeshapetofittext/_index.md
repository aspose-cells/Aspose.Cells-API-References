---
title: ChartTextFrame.IsResizeShapeToFitText
second_title: Aspose.Cells for .NET API Reference
description: ChartTextFrame property. Gets or sets whether a shape should be autofit to fully contain the text described within it. Autofitting is when text within a shape is scaled in order to contain all the text inside
type: docs
url: /net/aspose.cells.charts/charttextframe/isresizeshapetofittext/
---
## ChartTextFrame.IsResizeShapeToFitText property

Gets or sets whether a shape should be auto-fit to fully contain the text described within it. Auto-fitting is when text within a shape is scaled in order to contain all the text inside.

```csharp
public bool IsResizeShapeToFitText { get; set; }
```

### Examples

```csharp
// Called: point.DataLabels.IsResizeShapeToFitText = (false);
public void ChartTextFrame_Property_IsResizeShapeToFitText()
{
    String dataDir = Constants.destPath;
    // Create an instance of Workbook in XLSX format
    Workbook workbook = new Workbook(FileFormatType.Xlsx);

    // Access the first worksheet
    Worksheet worksheet = workbook.Worksheets[0];

    // Add two columns of data
    worksheet.Cells["A1"].PutValue("Retail");
    worksheet.Cells["A2"].PutValue("Services");
    worksheet.Cells["A3"].PutValue("Info & Communication");
    worksheet.Cells["A4"].PutValue("Transport Equip");
    worksheet.Cells["A5"].PutValue("Construction");

    worksheet.Cells["B1"].PutValue(98.0);
    worksheet.Cells["B2"].PutValue(0.5);
    worksheet.Cells["B3"].PutValue(0.5);
    worksheet.Cells["B4"].PutValue(0.5);
    worksheet.Cells["B5"].PutValue(0.5);

    // Create a pie chart and add it to the collection of charts
    int id = worksheet.Charts.Add(ChartType.Doughnut, 3, 3, 23, 10);
    // Access newly created Chart instance
    Chart chart = worksheet.Charts[id];

    // Set series data range
    chart.NSeries.Add("B1:B5", true);
    // Set category data range
    chart.NSeries.CategoryData = "A1:A5";
    // Turn off legend
    chart.ShowLegend = false;

    // Access data labels
    DataLabels dataLabels = chart.NSeries[0].DataLabels;
    // Turn on percentage format
    dataLabels.ShowPercentage = true;
    // Set position
    dataLabels.Position = LabelPositionType.OutsideEnd;

    //Turn on leader lines
    chart.NSeries[0].HasLeaderLines = true;

    //chart.getChartArea().getFont().setName("Century Gothic");
    chart.ChartArea.Font.Name = "Century Gothic";
    chart.ChartArea.Font.Size = 10;

    chart.ChartArea.Area.ForegroundColor = Color.FromArgb(0, 0, 0);
    chart.ChartArea.Area.Transparency = 1;
    chart.PlotArea.Area.ForegroundColor = Color.FromArgb(0, 0, 0);
    chart.PlotArea.Area.Transparency = 1;
    chart.ChartArea.Border.IsVisible = false;
    chart.PlotArea.Border.IsVisible = false;

    //Calculate chart
    ChartCalculateOptions calculateOptions = new ChartCalculateOptions();
    calculateOptions.UpdateAllPoints = true;
    chart.Calculate(calculateOptions);

    //You need to move DataLabels a little leftward or rightward depending on their position
    //to show leader lines
    int delta = 0;
    float minAngle = 10;
    double totalValue = 0;
    for (int i = 0; i < chart.NSeries[0].Points.Count; i++)
    {
        totalValue += Double.Parse(chart.NSeries[0].Points[i].YValue.ToString());
    }
    for (int i = chart.NSeries[0].Points.Count - 1; i >= 0; i--)
    {
        ChartPoint point = chart.NSeries[0].Points[i];

        point.DataLabels.IsResizeShapeToFitText = (false);
        point.DataLabels.IsTextWrapped = (false);

        point.DataLabels.NumberFormat = ("#0.00%");
        int X = point.DataLabels.X;
        int Y = point.DataLabels.Y;
        double val = Double.Parse(point.YValue.ToString());
        double angle = val / totalValue * 360;
        int deltaX = delta;
        int deltaY = -100;
        if (angle < minAngle)
        {
            int k = i + 1;
            while (k < chart.NSeries[0].Points.Count)
            {
                val += Double.Parse(chart.NSeries[0].Points[k].YValue.ToString());
                if (val / totalValue * 360 < minAngle)
                {
                    deltaX += 350;
                }
                deltaY += 100;
                k++;
            }

            // More offset is required for successive angles that are too small
            delta += 100;
        }
        else
        {
            delta = 0;
            if (angle > 2 * minAngle)
                deltaX = 0;
        }

        if (deltaX == 0 && angle > minAngle)
        {
            if (X > 2000)
            {
                point.DataLabels.X = (X + 350);
            }
            else
            {
                point.DataLabels.X = (X - 350);
            }
        }
        else if (deltaX > 0)
        {
            X -= deltaX;
            Y += deltaY;
            point.DataLabels.X = (X);
            point.DataLabels.Y = (Y);
        }
        else if (Y < 150)
        {
            // set label further away from chart to make the leader line show
            point.DataLabels.Y = (Y - 10);
        }
    }

    chart.Calculate();

    //In order to save the chart image, create an instance of ImageOrPrintOptions
    ImageOrPrintOptions anOption = new ImageOrPrintOptions();
    //Set image format
    anOption.ImageType = ImageType.Png;
    //Set resolution
    anOption.HorizontalResolution = 500;
    anOption.VerticalResolution = 500;

    //Render chart to image
    chart.ToImage(dataDir + "example.png", anOption);

    //Judging values
    Assert.AreEqual(chart.NSeries[0].Points.Count, 5);
    Assert.True(chart.NSeries[0].Points[0].DataLabels.Width > 350); //wrong:268, correct:429
    Assert.True(chart.NSeries[0].Points[1].DataLabels.Width > 280); //wrong:196, correct:366

    //Save the workbook to see chart inside the Excel
    workbook.Save(dataDir + "example.xlsx");
}
```

### See Also

* class [ChartTextFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


