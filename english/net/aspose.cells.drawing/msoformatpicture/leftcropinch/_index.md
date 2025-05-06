---
title: MsoFormatPicture.LeftCropInch
second_title: Aspose.Cells for .NET API Reference
description: MsoFormatPicture property. Represents the location of the left of the crop rectangle expressed in unit of inches
type: docs
url: /net/aspose.cells.drawing/msoformatpicture/leftcropinch/
---
## MsoFormatPicture.LeftCropInch property

Represents the location of the left of the crop rectangle expressed, in unit of inches.

```csharp
public double LeftCropInch { get; set; }
```

### Examples

```csharp
// Called: double x = pic.FormatPicture.LeftCropInch;
[Test]
        public void Property_LeftCropInch()
        {
            var workbook = new Aspose.Cells.Workbook();
            var sheet = workbook.Worksheets[0];
            var bmpBytes = File.ReadAllBytes(Constants.sourcePath + &quot;CELLSNET-54285.png&quot;);
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


