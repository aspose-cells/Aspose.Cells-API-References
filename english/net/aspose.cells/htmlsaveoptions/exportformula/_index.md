---
title: HtmlSaveOptions.ExportFormula
second_title: Aspose.Cells for .NET API Reference
description: HtmlSaveOptions property. Indicates whether exporting formula when saving file to html. The default value is true. If you want to import the output html to excel please keep the default value
type: docs
url: /net/aspose.cells/htmlsaveoptions/exportformula/
---
## HtmlSaveOptions.ExportFormula property

Indicates whether exporting formula when saving file to html. The default value is true. If you want to import the output html to excel, please keep the default value.

```csharp
public bool ExportFormula { get; set; }
```

### Examples

```csharp
// Called: options.ExportFormula = (false);
[Test]
        public void Property_ExportFormula()
        {
            Workbook wb = new Workbook(Constants.HtmlPath + &quot;CELLSJAVA-45550.xlsx&quot;);


            // Initialize HtmlSaveOptions
            HtmlSaveOptions options = new HtmlSaveOptions(SaveFormat.Html);

            prepareRangeForExport(wb, &quot;VerticalText_Cell&quot;);


            // Specify the HTML Saving Options
            // IMPORTANT: Set the encoding to UTF8 so that non-ASCII characters in the range
            // are generated properly.
            options.Encoding = (Encoding.UTF8);

            // Note use HtmlCrossType.CROSS since DEFAULT can produce unwanted results in
            // some scenarios
            options.HtmlCrossStringType = (HtmlCrossType.Cross);
            options.PresentationPreference = (true); // suposedly creates a &apos;more beautiful presentation&apos;
            options.ExportHiddenWorksheet = (false);
            options.ExportActiveWorksheetOnly = (true);
            options.ExportImagesAsBase64 = (true); // avoids the temp folder
            options.CreateDirectory = (false);
            options.IsExpImageToTempDir = (false);
            options.HiddenColDisplayType = (HtmlHiddenColDisplayType.Remove);
            options.HiddenRowDisplayType = (HtmlHiddenRowDisplayType.Remove);

            // The following options reduce the size of the generated HTML (without impacting quality)
            options.ExportFormula = (false);
            options.ExcludeUnusedStyles = (true);

            options.ExportBogusRowData = (false);
            options.ExportFrameScriptsAndProperties = (false);

            ImageOrPrintOptions imgOptions = options.ImageOptions;
            imgOptions.ImageType = (ImageType.Svg);

            wb.Save(_destFilesPath + &quot;CELLSJAVA-45550.html&quot;, options);
            Workbook wb2 = new Workbook(_destFilesPath + &quot;CELLSJAVA-45550.html&quot;);
            Cells cells = wb2.Worksheets[0].Cells;
            Assert.AreEqual(cells[&quot;b4&quot;].DisplayStringValue, &quot;Item 2&quot;);
            Assert.AreEqual(cells[&quot;b12&quot;].DisplayStringValue, &quot;Item 10&quot;);

        }
```

### See Also

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


