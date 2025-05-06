---
title: ImageSaveOptions.StreamProvider
second_title: Aspose.Cells for .NET API Reference
description: ImageSaveOptions property. Gets or sets the IStreamProvider for exporting objects
type: docs
url: /net/aspose.cells/imagesaveoptions/streamprovider/
---
## ImageSaveOptions.StreamProvider property

Gets or sets the IStreamProvider for exporting objects.

```csharp
public IStreamProvider StreamProvider { get; set; }
```

### Remarks

If saving as Tiff, this property is ignored. Otherwise, if more than one image should be saving, we will write other images by this. For advanced usage, please use [`WorkbookRender`](../../../aspose.cells.rendering/workbookrender/) or [`SheetRender`](../../../aspose.cells.rendering/sheetrender/).

### Examples

```csharp
// Called: saveOptions.StreamProvider = new StreamProvider();
[Test]
        public void Property_StreamProvider()
        {

            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CELLSNET49614.xlsx&quot;);
         
            workbook.Save(Constants.destPath + &quot;CELLSNET49614.png&quot;);
            Assert.AreEqual(FileFormatType.Png, FileFormatUtil.DetectFileFormat(Constants.destPath + &quot;CELLSNET49614.png&quot;).FileFormatType);
            ImageSaveOptions saveOptions = new ImageSaveOptions(SaveFormat.Png);
            saveOptions.StreamProvider = new StreamProvider();
            workbook.Save(Constants.destPath + &quot;CELLSNET49614.png&quot;, saveOptions);
            Assert.AreEqual(FileFormatType.Png, FileFormatUtil.DetectFileFormat(Constants.destPath + &quot;CELLSNET49614.png&quot;).FileFormatType);
            //Assert.IsTrue(File.Exists(Constants.destPath + &quot;1.png&quot;));
        }
```

### See Also

* interface [IStreamProvider](../../istreamprovider/)
* class [ImageSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


