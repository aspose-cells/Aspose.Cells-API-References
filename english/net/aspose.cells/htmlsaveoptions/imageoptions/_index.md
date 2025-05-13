---
title: HtmlSaveOptions.ImageOptions
second_title: Aspose.Cells for .NET API Reference
description: HtmlSaveOptions property. Get the ImageOrPrintOptions object before exporting
type: docs
url: /net/aspose.cells/htmlsaveoptions/imageoptions/
---
## HtmlSaveOptions.ImageOptions property

Get the ImageOrPrintOptions object before exporting

```csharp
public ImageOrPrintOptions ImageOptions { get; }
```

### Examples

```csharp
// Called: ImageOrPrintOptions imageOptions = options.ImageOptions;
public void HtmlSaveOptions_Property_ImageOptions()
{
    Workbook wb = new Workbook(Constants.HtmlPath + "example.xlsx");
    HtmlSaveOptions options = new HtmlSaveOptions();
    options.ExportPrintAreaOnly = true;
    options.ExportImagesAsBase64 = true;
    ImageOrPrintOptions imageOptions = options.ImageOptions;
    imageOptions.ImageType = ImageType.Svg;
    wb.Save(_destFilesPath + "example.html", options);

    string dir = _destFilesPath + "CELLSJAVA-44534_files";
    DirectoryInfo dirInfo = new DirectoryInfo(dir);

    foreach (FileInfo fileInfo in dirInfo.GetFiles())
    {
        if (fileInfo.Extension == ".htm" && fileInfo.Name.IndexOf("sheet") > -1)
        {
            string content = File.ReadAllText(fileInfo.FullName);
            Assert.IsTrue(content.IndexOf("<svg") > -1);
        }
    }
}
```

### See Also

* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


