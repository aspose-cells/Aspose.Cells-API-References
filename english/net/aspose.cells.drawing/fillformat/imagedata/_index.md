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
// Called: comment3.CommentShape.Fill.ImageData = imgData3;
public void FillFormat_Property_ImageData()
{
    Workbook wb3 = new Workbook();
    Worksheet sheet3 = wb3.Worksheets[0];
    sheet3.Pictures.Add(0, 0, Constants.sourcePath + @"example.png");
    var comment3 = sheet3.Comments[sheet3.Comments.Add(2, 15)];
    var imgData3 = File.ReadAllBytes(Constants.sourcePath + @"example.png");
    comment3.CommentShape.Fill.ImageData = imgData3;

    comment3 = sheet3.Comments[sheet3.Comments.Add(6, 15)];
    comment3.CommentShape.Fill.ImageData = imgData3;
    using(MemoryStream s  = new MemoryStream())
    {
        wb3.Save(s, SaveFormat.Xlsx);
        s.Flush();
        s.Seek(0, SeekOrigin.Begin);

       Assert.IsFalse( ManualFileUtil.ContainsEntry(s, "xl/media/image2.png"));

    }
          
}
```

### See Also

* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


