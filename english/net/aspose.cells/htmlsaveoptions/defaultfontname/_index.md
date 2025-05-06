---
title: HtmlSaveOptions.DefaultFontName
second_title: Aspose.Cells for .NET API Reference
description: HtmlSaveOptions property. Specify the default font name for exporting html the default font will be used when the font of style is not existing If this property is null Aspose.Cells will use universal font which have the same family with the original font the default value is null
type: docs
url: /net/aspose.cells/htmlsaveoptions/defaultfontname/
---
## HtmlSaveOptions.DefaultFontName property

Specify the default font name for exporting html, the default font will be used when the font of style is not existing, If this property is null, Aspose.Cells will use universal font which have the same family with the original font, the default value is null.

```csharp
public string DefaultFontName { get; set; }
```

### Examples

```csharp
// Called: saveOptions.DefaultFontName = null;
[Test]
        public void Property_DefaultFontName()
        {
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.ExportPrintAreaOnly = true;
            saveOptions.ExportActiveWorksheetOnly = true;
            saveOptions.ExportImagesAsBase64 = true;
            saveOptions.ExportDataOptions = HtmlExportDataOptions.All;
            saveOptions.DefaultFontName = null;
            saveOptions.IsExportComments = false;
            saveOptions.ExportRowColumnHeadings = false;
            saveOptions.ExportExtraHeadings = true;
            saveOptions.ExportGridLines = false;
            saveOptions.HtmlCrossStringType = HtmlCrossType.Default;
            saveOptions.CellCssPrefix = &quot;p1-65dd5c19f29-&quot;;

            Workbook wb = new Workbook(Constants.HtmlPath + &quot;CELLSNET-56578.xlsx&quot;);
            WorksheetCollection sheets = wb.Worksheets;
            string destPath = _destFilesPath + &quot;CELLSNET-56578&quot;;
            if (!Directory.Exists(destPath))
                Directory.CreateDirectory(destPath);
            for (int i = 0; i &lt; sheets.Count; i++)// sheets.Count is growing in trial mode
            {
                Worksheet one = sheets[i];
                saveOptions.TableCssId = &quot;gdt-id-&quot; + (i + 1).ToString();
                one.IsSelected = true;
                wb.Worksheets.ActiveSheetIndex = one.Index;
                Console.WriteLine(&quot;Saving worksheet {0} - &apos;{1}&apos;&quot;, one.Index, one.Name);
                string outputFilename = destPath + string.Format(&quot;CELLSNET-56578_{0}_{1}.html&quot;, one.Index, one.Name);
                wb.Save(outputFilename, saveOptions); // exception here
            }
        }
```

### See Also

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


