---
title: Picture.SourceFullName
second_title: Aspose.Cells for .NET API Reference
description: Picture property. Gets or sets the path and name of the source file for the linked image
type: docs
url: /net/aspose.cells.drawing/picture/sourcefullname/
---
## Picture.SourceFullName property

Gets or sets the path and name of the source file for the linked image.

```csharp
public string SourceFullName { get; set; }
```

### Remarks

The default value is an empty string. If SourceFullName is not an empty string, the image is linked. If SourceFullName is not an empty string, but Data is null, then the image is linked and not stored in the file.

### Examples

```csharp
// Called: Assert.IsTrue(!string.IsNullOrEmpty(pics[0].SourceFullName));
public void Picture_Property_SourceFullName()
{

    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    PictureCollection pics = workbook.Worksheets[0].Pictures;
    // Picture pic =  workbook.Worksheets[0].Shapes.AddLinkedPicture(0, 0, 100, 100, dir + "image1.png");
    Assert.AreEqual(ImageType.Svg, pics[0].ImageType);
    Assert.IsTrue(pics[0].IsLink);
    Assert.IsTrue(!string.IsNullOrEmpty(pics[0].SourceFullName));
    workbook.Save(Constants.destPath + "example.xlsx");
}
```

### See Also

* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


