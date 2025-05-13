---
title: HtmlSaveOptions.ExportPageHeaders
second_title: Aspose.Cells for .NET API Reference
description: HtmlSaveOptions property. Indicates whether exporting page headers
type: docs
url: /net/aspose.cells/htmlsaveoptions/exportpageheaders/
---
## HtmlSaveOptions.ExportPageHeaders property

Indicates whether exporting page headers.

```csharp
public bool ExportPageHeaders { get; set; }
```

### Remarks

Only works when [`SaveAsSingleFile`](../saveassinglefile/) is True.

### Examples

```csharp
// Called: saveOptions.ExportPageHeaders = true;
public void HtmlSaveOptions_Property_ExportPageHeaders()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    HtmlSaveOptions saveOptions = new HtmlSaveOptions();
    saveOptions.SaveAsSingleFile = true;
    saveOptions.ShowAllSheets = true;

    saveOptions.ExportPageHeaders = true;
         
    workbook.Save(Constants.destPath + "example.html", saveOptions);
    string text = File.ReadAllText(Constants.destPath + "example.html");
    Assert.IsTrue(text.IndexOf("Sheet 1 - Summary") != -1);
}
```

### See Also

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


