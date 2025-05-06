---
title: Worksheet.Pictures
second_title: Aspose.Cells for .NET API Reference
description: Worksheet property. Gets a Picture collection
type: docs
url: /net/aspose.cells/worksheet/pictures/
---
## Worksheet.Pictures property

Gets a [`Picture`](../../../aspose.cells.drawing/picture/) collection.

```csharp
public PictureCollection Pictures { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(1, reloadWb.Worksheets[0].Pictures.Count);
[Test]
        public void Property_Pictures()
        {
            HtmlSaveOptions htmlSaveOptions = new HtmlSaveOptions();
            htmlSaveOptions.ExportActiveWorksheetOnly = true;

            Workbook wb = new Workbook(Constants.HtmlPath + &quot;CELLSJAVA-43853.xlsx&quot;);
            string savePath = _destFilesPath + &quot;CELLSJAVA-43853_07.html&quot;;

            wb.Save(savePath, htmlSaveOptions);

            Workbook reloadWb = new Workbook(savePath);
            Assert.AreEqual(1, reloadWb.Worksheets[0].Pictures.Count);
            Assert.AreEqual(ImageType.Png, reloadWb.Worksheets[0].Pictures[0].ImageType);


            htmlSaveOptions.ExportImagesAsBase64 = true;
            savePath = _destFilesPath + &quot;CELLSJAVA-43853_07_base64.html&quot;;

            wb.Save(savePath, htmlSaveOptions);

            reloadWb = new Workbook(savePath);
            Assert.AreEqual(1, reloadWb.Worksheets[0].Pictures.Count);
            Assert.AreEqual(ImageType.Png, reloadWb.Worksheets[0].Pictures[0].ImageType);
        }
```

### See Also

* class [PictureCollection](../../../aspose.cells.drawing/picturecollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


