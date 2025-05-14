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
// Called: options.CellCssPrefix = "prefix";
private void HtmlSaveOptions_Property_CellCssPrefix(string filePath, string fileName)
        {
            Workbook wb = new Workbook(filePath + fileName);
            Worksheet ws = wb.Worksheets[0];

            wb.Worksheets.ActiveSheetIndex = 0;
            ws.PageSetup.PrintArea = "A1:N50";

            HtmlSaveOptions options = new HtmlSaveOptions();
            options.ExportPrintAreaOnly = true;
            options.ExportActiveWorksheetOnly = true;
            options.ExportImagesAsBase64 = true;
            options.ExportDataOptions = HtmlExportDataOptions.All;
            options.CellCssPrefix = "prefix";

           
            wb.Save(_destFilesPath + "example.html", options);
        }
```

### See Also

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


