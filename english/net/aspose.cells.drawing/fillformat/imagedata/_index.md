---
title: FillFormat.ImageData
second_title: Aspose.Cells for .NET API Reference
description: FillFormat property. Gets and sets the picture image data
type: docs
url: /net/aspose.cells.drawing/fillformat/imagedata/
---
## FillFormat.ImageData property

Gets and sets the picture image data.

```csharp
public byte[] ImageData { get; set; }
```

### Remarks

If the fill format is not custom texture format, returns null.

### Examples

```csharp
// Called: comment.CommentShape.Fill.ImageData = imgData;
[Test]
        public void Property_ImageData()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            var comment = sheet.Comments[sheet.Comments.Add(0, 0)];
            var imgData = File.ReadAllBytes(Constants.sourcePath + @&quot;CELLSNET-54285.png&quot;);
            comment.CommentShape.Fill.ImageData = imgData;
            //now the RelativeToOriginalPictureSize is true, WidthScale and HeightScale are 100
            //belows setter not change anything and do nothing at all.
            comment.CommentShape.RelativeToOriginalPictureSize = true;
            comment.CommentShape.WidthScale = 100;
            comment.CommentShape.HeightScale = 100;

            MemoryStream stream = new MemoryStream(imgData);
            Image img = Image.FromStream(stream);
            Assert.AreEqual(img.Width, (int)(comment.CommentShape.Width /CellsHelper.DPI * 120 + 0.5));
            Assert.AreEqual(img.Height, (int)(comment.CommentShape.Height / CellsHelper.DPI * 120 + 0.5));
            wb.Save(Constants.destPath + &quot;CELLSNET54285.xlsx&quot;);
            wb = new Workbook(Constants.destPath + &quot;CELLSNET54285.xlsx&quot;);
            Assert.IsTrue(wb.Worksheets[0].Comments[0].CommentShape.RelativeToOriginalPictureSize);
        }
```

### See Also

* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


