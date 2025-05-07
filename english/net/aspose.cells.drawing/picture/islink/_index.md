---
title: Picture.IsLink
second_title: Aspose.Cells for .NET API Reference
description: Picture property. Returns true if the picture is linked to a file
type: docs
url: /net/aspose.cells.drawing/picture/islink/
---
## Picture.IsLink property

Returns true if the picture is linked to a file.

```csharp
public bool IsLink { get; set; }
```

### Examples

```csharp
// Called: Assert.IsTrue(pics[0].IsLink);
[Test]
        public void Property_IsLink()
        {

            Workbook workbook = new Workbook(Constants.sourcePath + "CellsNet47362.xlsx");
            PictureCollection pics = workbook.Worksheets[0].Pictures;
            // Picture pic =  workbook.Worksheets[0].Shapes.AddLinkedPicture(0, 0, 100, 100, dir + "image1.png");
            Assert.AreEqual(ImageType.Svg, pics[0].ImageType);
            Assert.IsTrue(pics[0].IsLink);
            Assert.IsTrue(!string.IsNullOrEmpty(pics[0].SourceFullName));
            workbook.Save(Constants.destPath + "CellsNet47362.xlsx");
        }
```

### See Also

* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


