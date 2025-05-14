---
title: StreamProviderOptions.CustomPath
second_title: Aspose.Cells for .NET API Reference
description: StreamProviderOptions property. The user custom pathURL saved in generated html file for the referred source. If not defined by user DefaultPath will be used. For example the sheet data will be saved by user to d/sheet001.htm the url used in the main html file should be d/sheet001.htm or other valid relative path that can be accessed by the main html file
type: docs
url: /net/aspose.cells/streamprovideroptions/custompath/
---
## StreamProviderOptions.CustomPath property

The user custom path(URL) saved in generated html file for the referred source. If not defined by user, DefaultPath will be used. For example, the sheet data will be saved by user to d:/sheet001.htm, the url used in the main html file should be "d:/sheet001.htm" or other valid relative path that can be accessed by the main html file.

```csharp
public string CustomPath { get; set; }
```

### Examples

```csharp
// Called: Assert.IsTrue(File.Exists(Path.Combine(streamProvider._outputDirectory, streamProvider.streamProviderOptions.CustomPath)));
public void StreamProviderOptions_Property_CustomPath()
{
    Workbook wb = new Workbook(Constants.HtmlPath + "example.xlsx");
    wb.Worksheets.ActiveSheetIndex = 0;
    HtmlSaveOptions options = new HtmlSaveOptions();
    options.ExportActiveWorksheetOnly = true;
    options.ExportDataOptions = HtmlExportDataOptions.All;
    HtmlWithExternalResourcesProvider streamProvider = new HtmlWithExternalResourcesProvider(_destFilesPath);
    options.StreamProvider = streamProvider;
    options.IsExpImageToTempDir = false;

    string outputFile = Path.Combine(_destFilesPath, "example.html");
    using (FileStream fs = new FileStream(outputFile, FileMode.Create))
    {
        wb.Save(fs, options);
    }
    string text = File.ReadAllText(outputFile);
    Assert.IsTrue(text.IndexOf("width:113px;height:45px'><img width='113' height='45'") > -1);
    Assert.IsTrue(File.Exists(Path.Combine(streamProvider._outputDirectory, streamProvider.streamProviderOptions.CustomPath)));
}
```

### See Also

* class [StreamProviderOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


