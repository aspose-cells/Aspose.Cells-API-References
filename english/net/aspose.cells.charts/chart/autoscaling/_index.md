---
title: Chart.AutoScaling
second_title: Aspose.Cells for .NET API Reference
description: Chart property. True if Microsoft Excel scales a 3D chart so that its closer in size to the equivalent 2D chart. The RightAngleAxes property must be True
type: docs
url: /net/aspose.cells.charts/chart/autoscaling/
---
## Chart.AutoScaling property

True if Microsoft Excel scales a 3-D chart so that it's closer in size to the equivalent 2-D chart. The RightAngleAxes property must be True.

```csharp
public bool AutoScaling { get; set; }
```

### Examples

```csharp
// Called: chart.AutoScaling = false;
public void Chart_Property_AutoScaling()
{
    string path = Constants.TemplatePath + "NetCoreTests/CELLSNETCORE53/";
    string fileName = "input_green_dot_test.xlsx";
    string filePathName = path + fileName;
    string savedFile = destPathNetCore + "input_green_dot_test.pdf";

    Workbook sourceBook = new Workbook(filePathName);
    foreach (Aspose.Cells.Charts.Chart chart in sourceBook.Worksheets[0].Charts)
    {
        chart.PrintSize = PrintSizeType.Full;
        chart.SizeWithWindow = false;
        chart.AutoScaling = false;
        int width = chart.GapWidth;
        chart.GapWidth = 100;
        //chart.PageSetup.Zoom;
    }
    SaveOptions so = new PdfSaveOptions();
    so.ValidateMergedAreas = true;
    so.RefreshChartCache = true;
    so.MergeAreas = true;
    sourceBook.Save(savedFile, so);

}
```

### See Also

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


