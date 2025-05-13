---
title: GlobalizationSettings.ChartSettings
second_title: Aspose.Cells for .NET API Reference
description: GlobalizationSettings property. Gets or sets the globalization settings for Chart
type: docs
url: /net/aspose.cells/globalizationsettings/chartsettings/
---
## GlobalizationSettings.ChartSettings property

Gets or sets the globalization settings for Chart.

```csharp
public ChartGlobalizationSettings ChartSettings { get; set; }
```

### Examples

```csharp
// Called: book.Settings.GlobalizationSettings.ChartSettings = new TestChartGlobalizationSetttings();
public void GlobalizationSettings_Property_ChartSettings()
{
    var book = new Workbook(Constants.sourcePath + "Xl_V2.xlsx");
    CellsHelper.DPI = 96;
    book.Settings.CultureInfo = new System.Globalization.CultureInfo("es-ES");

    ///////////////////
    //Add this line
    book.Settings.GlobalizationSettings.ChartSettings = new TestChartGlobalizationSetttings();
    //////////////////
    Worksheet excelWorksheet = book.Worksheets["Hoja1"];
    Aspose.Cells.Range range = excelWorksheet.Workbook.Worksheets.GetRangeByName("BIPLI_PRUEBA_CASCADA");
    string startCell = CellsHelper.CellIndexToName(range.FirstRow, range.FirstColumn);
    string endCell = CellsHelper.CellIndexToName(range.FirstRow + range.RowCount - 1, range.FirstColumn + range.ColumnCount - 1);
    string rangeAddress = string.Format("{0}:{1}", startCell, endCell);

    ImageOrPrintOptions options = new ImageOrPrintOptions();
    options.AllColumnsInOnePagePerSheet = true;
    options.ImageType = Aspose.Cells.Drawing.ImageType.Png;
    options.OnePagePerSheet = true;
    options.HorizontalResolution = 600;
    options.VerticalResolution = 600;
    options.OnlyArea = true;

    Aspose.Cells.PageSetup pageSetup = excelWorksheet.PageSetup;


    pageSetup.PrintArea = rangeAddress;
    using (MemoryStream imageStream = new MemoryStream())
    {
        SheetRender sr = new SheetRender(excelWorksheet, options);
        //sr.ToImage(0, imageStream);
        //Image.FromStream(imageStream).Save(Constants.destPath + "example.png", ImageFormat.Png);
        sr.ToImage(0, Constants.destPath + "example.png");

    };
}
```

### See Also

* class [ChartGlobalizationSettings](../../../aspose.cells.charts/chartglobalizationsettings/)
* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


