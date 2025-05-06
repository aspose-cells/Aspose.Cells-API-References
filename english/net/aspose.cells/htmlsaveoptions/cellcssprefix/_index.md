---
title: HtmlSaveOptions.CellCssPrefix
second_title: Aspose.Cells for .NET API Reference
description: HtmlSaveOptions property. Gets and sets the prefix of the css namethe default value is 
type: docs
url: /net/aspose.cells/htmlsaveoptions/cellcssprefix/
---
## HtmlSaveOptions.CellCssPrefix property

Gets and sets the prefix of the css name,the default value is "".

```csharp
public string CellCssPrefix { get; set; }
```

### Examples

```csharp
// Called: options.CellCssPrefix = &amp;quot;prefix&amp;quot;;
private void Property_CellCssPrefix(string filePath, string fileName)
        {
            Workbook wb = new Workbook(filePath + fileName);
            Worksheet ws = wb.Worksheets[0];

            wb.Worksheets.ActiveSheetIndex = 0;
            ws.PageSetup.PrintArea = &quot;A1:N50&quot;;

            HtmlSaveOptions options = new HtmlSaveOptions();
            options.ExportPrintAreaOnly = true;
            options.ExportActiveWorksheetOnly = true;
            options.ExportImagesAsBase64 = true;
            options.ExportDataOptions = HtmlExportDataOptions.All;
            options.CellCssPrefix = &quot;prefix&quot;;

           
            wb.Save(_destFilesPath + &quot;NET47653_PrintArea.html&quot;, options);
        }
```

### See Also

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


