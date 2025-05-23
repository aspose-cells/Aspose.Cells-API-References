---
title: Chart.PlotVisibleCellsOnly
second_title: Aspose.Cells for .NET API Reference
description: Chart property. Indicates whether plot visible cells only
type: docs
url: /net/aspose.cells.charts/chart/plotvisiblecellsonly/
---
## Chart.PlotVisibleCellsOnly property

Indicates whether plot visible cells only.

```csharp
public bool PlotVisibleCellsOnly { get; set; }
```

### Examples

```csharp
// Called: workbook.Worksheets["Data"].Charts[0].PlotVisibleCellsOnly = false;
public void Chart_Property_PlotVisibleCellsOnly()
{
    string filePath = Constants.JohnTest_PATH_SOURCE + @"JAVA41378/";
    Workbook workbook = new Workbook(filePath + "Xls_To_HTML_Test.XLSX");

    Worksheet worksheet = workbook.Worksheets[0];
    Cells cells = worksheet.Cells;
    HtmlSaveOptions saveOptions = new HtmlSaveOptions(SaveFormat.Html);
    saveOptions.ImageOptions.ImageType = ImageType.Png;
    saveOptions.ImageOptions.Transparent = true;
    saveOptions.ExportHiddenWorksheet = false;
    saveOptions.PresentationPreference = true;

    //saveOptions.getImageOptions().setRenderingHint(RenderingHints.KEY_ANTIALIASING, RenderingHints.VALUE_ANTIALIAS_ON);

    //saveOptions.getImageOptions().setRenderingHint(RenderingHints.KEY_TEXT_ANTIALIASING, RenderingHints.VALUE_TEXT_ANTIALIAS_ON);

    PageSetup pgSetup = workbook.Worksheets[0].PageSetup;
    pgSetup.PrintArea = "A1:BU43";
    saveOptions.HiddenRowDisplayType = HtmlHiddenRowDisplayType.Hidden;
    workbook.Worksheets["Data"].Charts[0].PlotVisibleCellsOnly = false;
    workbook.Save(CreateFolder(filePath) + "out.html", saveOptions);
}
```

### See Also

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


