---
title: HtmlSaveOptions.StreamProvider
second_title: Aspose.Cells for .NET API Reference
description: HtmlSaveOptions property. Gets or sets the IStreamProvider for exporting objects
type: docs
url: /net/aspose.cells/htmlsaveoptions/streamprovider/
---
## HtmlSaveOptions.StreamProvider property

Gets or sets the IStreamProvider for exporting objects.

```csharp
public IStreamProvider StreamProvider { get; set; }
```

### Examples

```csharp
// Called: options.StreamProvider = new ExportStreamProvider(outputDir);
public void HtmlSaveOptions_Property_StreamProvider()
{
    ;
    string filePath = Constants.JohnTest_PATH_SOURCE + @"NET43262/";
    string savePath = CreateFolder(filePath);

    string outputDir = savePath + @"out/";
    Workbook wb = new Workbook(filePath + "a.xlsx");
    HtmlSaveOptions options = new HtmlSaveOptions();
    options.ExportActiveWorksheetOnly = true;
    options.StreamProvider = new ExportStreamProvider(outputDir);
    wb.Save(savePath + "out.html", options);
}
```

### See Also

* interface [IStreamProvider](../../istreamprovider/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


