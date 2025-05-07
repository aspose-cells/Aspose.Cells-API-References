---
title: MsoFormatPicture.LeftCrop
second_title: Aspose.Cells for .NET API Reference
description: MsoFormatPicture property. Represents the location of the left of the crop rectangle expressed expressed as a ratio of the images width
type: docs
url: /net/aspose.cells.drawing/msoformatpicture/leftcrop/
---
## MsoFormatPicture.LeftCrop property

Represents the location of the left of the crop rectangle expressed, expressed as a ratio of the image's width.

```csharp
public double LeftCrop { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(Math.Round(pic.FormatPicture.LeftCrop, 1), 0.1);
[Test]
        public void Property_LeftCrop()
        {
            var workbook = new Aspose.Cells.Workbook();
            var sheet = workbook.Worksheets[0];
            var bmpBytes = File.ReadAllBytes(Constants.sourcePath + "CELLSNET-54285.png");
            var picId = sheet.Pictures.Add(0, 0, new MemoryStream(bmpBytes));
            var pic = sheet.Pictures[picId];
            pic.FormatPicture.LeftCrop = 0.1;

            pic.FormatPicture.TopCrop = 0.1;
            double x = pic.FormatPicture.LeftCropInch;

            pic.FormatPicture.LeftCropInch = x;
            Assert.AreEqual(Math.Round(pic.FormatPicture.LeftCrop, 1), 0.1);

        }
```

### See Also

* class [MsoFormatPicture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


