---
title: Chart.SizeWithWindow
second_title: Aspose.Cells for .NET API Reference
description: Chart property. True if Microsoft Excel resizes the chart to match the size of the chart sheet window
type: docs
url: /net/aspose.cells.charts/chart/sizewithwindow/
---
## Chart.SizeWithWindow property

True if Microsoft Excel resizes the chart to match the size of the chart sheet window.

```csharp
public bool SizeWithWindow { get; set; }
```

### Examples

```csharp
// Called: chart.SizeWithWindow = false;
[Test]
        public void Property_SizeWithWindow()
        {
            string path = Constants.TemplatePath + &quot;NetCoreTests/CELLSNETCORE53/&quot;;
            string fileName = &quot;input_green_dot_test.xlsx&quot;;
            string filePathName = path + fileName;
            string savedFile = destPathNetCore + &quot;input_green_dot_test.pdf&quot;;

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


