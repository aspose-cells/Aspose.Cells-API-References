---
title: HtmlSaveOptions.AddGenericFont
second_title: Aspose.Cells for .NET API Reference
description: HtmlSaveOptions property. Indicates whether to add a generic font to CSS fontfamily. The default value is true
type: docs
url: /net/aspose.cells/htmlsaveoptions/addgenericfont/
---
## HtmlSaveOptions.AddGenericFont property

Indicates whether to add a generic font to CSS font-family. The default value is true

```csharp
public bool AddGenericFont { get; set; }
```

### Examples

```csharp
// Called: options.AddGenericFont = false;
public void HtmlSaveOptions_Property_AddGenericFont()
{
    Workbook wb = new Workbook(Constants.HtmlPath + "example.xlsx"); 
    Aspose.Cells.Range range = wb.Worksheets.GetRangeByName("PIANETI");
    Worksheet ws = range.Worksheet;
    PageSetup pageSetup = ws.PageSetup;
    pageSetup.PrintArea = (range.Address);
    HtmlSaveOptions options = new HtmlSaveOptions(SaveFormat.Html);
    options.ExportPrintAreaOnly = true;
    options.ExportBogusRowData = false;
    wb.Save(_destFilesPath + "example.html", options);
    string text = File.ReadAllText(_destFilesPath + "example.html");
    Assert.IsTrue(text.IndexOf("font-family:Pacifico,sans-serif;") > -1);
    options.AddGenericFont = false;
    wb.Save(_destFilesPath + "example.html", options);
    text = File.ReadAllText(_destFilesPath + "example.html");
    Assert.IsTrue(text.IndexOf("font-family:Pacifico,sans-serif;") == -1);
}
```

### See Also

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


