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
[Test]
        public void Property_ChartSettings()
        {
            var book = new Workbook(Constants.sourcePath + &quot;Xl_V2.xlsx&quot;);
            CellsHelper.DPI = 96;
            book.Settings.CultureInfo = new System.Globalization.CultureInfo(&quot;es-ES&quot;);

            ///////////////////
            //Add this line
            book.Settings.GlobalizationSettings.ChartSettings = new TestChartGlobalizationSetttings();
            //////////////////
            Worksheet excelWorksheet = book.Worksheets[&quot;Hoja1&quot;];
            Aspose.Cells.Range range = excelWorksheet.Workbook.Worksheets.GetRangeByName(&quot;BIPLI_PRUEBA_CASCADA&quot;);
            string startCell = CellsHelper.CellIndexToName(range.FirstRow, range.FirstColumn);
            string endCell = CellsHelper.CellIndexToName(range.FirstRow + range.RowCount - 1, range.FirstColumn + range.ColumnCount - 1);
            string rangeAddress = string.Format(&quot;{0}:{1}&quot;, startCell, endCell);

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
                //Image.FromStream(imageStream).Save(Constants.destPath + &quot;Charts2Image/CELLSNET52029.png&quot;, ImageFormat.Png);
                sr.ToImage(0, Constants.destPath + &quot;Charts2Image/CELLSNET52029.png&quot;);

            };
        }
```

### See Also

* class [ChartGlobalizationSettings](../../../aspose.cells.charts/chartglobalizationsettings/)
* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


