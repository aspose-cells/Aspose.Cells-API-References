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
// Called: saveOptions.ImageOptions.ImageType = ImageType.Jpeg;
[Test]
        public void Property_ImageOptions()
        {
            string filePath = Constants.JohnTest_PATH_SOURCE + @"NET45073/";

            string exportPath = Constants.JohnTest_PATH_SOURCE + @"NET45073\aa/";
            CreateFolder(filePath);
            exportPath = CreateFolder(exportPath);

            FileStream stream = File.OpenRead(filePath + "Test2.xlsx");
            Workbook workbook = new Workbook(stream);
            HtmlSaveOptions saveOptions = new HtmlSaveOptions(SaveFormat.Html);
            saveOptions.ParseHtmlTagInCell = true;
            saveOptions.ImageOptions.ImageType = ImageType.Jpeg;
            saveOptions.StreamProvider = new ExportStreamProvider(exportPath);
            Stream tempStream = new MemoryStream();
            workbook.Save(tempStream, saveOptions);
        }
```

### See Also

* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


