---
title: HtmlSaveOptions.ExportPrintAreaOnly
second_title: Aspose.Cells for .NET API Reference
description: HtmlSaveOptions property. Indicates if only exporting the print area to html file. The default value is false
type: docs
url: /net/aspose.cells/htmlsaveoptions/exportprintareaonly/
---
## HtmlSaveOptions.ExportPrintAreaOnly property

Indicates if only exporting the print area to html file. The default value is false.

```csharp
public bool ExportPrintAreaOnly { get; set; }
```

### Examples

```csharp
// Called: options.ExportPrintAreaOnly = true;
public void HtmlSaveOptions_Property_ExportPrintAreaOnly()
{
    string filePath = Constants.JohnTest_PATH_SOURCE + @"NET47871/";
    string savePath = CreateFolder(filePath);

    Workbook wb = new Workbook(filePath + "sample.xlsx");
    Worksheet ws = wb.Worksheets[0];

    ws.PageSetup.PrintArea = "J1:R18";

    HtmlSaveOptions options = new HtmlSaveOptions();
    options.ExportDataOptions = HtmlExportDataOptions.All;
    options.ExportImagesAsBase64 = true;
    options.ExportHeadings = true;
    options.ExportPrintAreaOnly = true;
    options.ExportGridLines = true;

    wb.Save(savePath + "out.html", options);
}
```

### See Also

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


