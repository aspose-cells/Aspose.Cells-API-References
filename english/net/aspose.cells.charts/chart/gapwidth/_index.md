---
title: Chart.GapWidth
second_title: Aspose.Cells for .NET API Reference
description: Chart property. Returns or sets the space between bar or column clusters as a percentage of the bar or column width. The value of this property must be between 0 and 500
type: docs
url: /net/aspose.cells.charts/chart/gapwidth/
---
## Chart.GapWidth property

Returns or sets the space between bar or column clusters, as a percentage of the bar or column width. The value of this property must be between 0 and 500.

```csharp
public int GapWidth { get; set; }
```

### Examples

```csharp
// Called: int width = chart.GapWidth;
public void Chart_Property_GapWidth()
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


