---
title: MsoFormatPicture.TransparentColor
second_title: Aspose.Cells for .NET API Reference
description: MsoFormatPicture property. Gets and sets the transparent color of the picture
type: docs
url: /net/aspose.cells.drawing/msoformatpicture/transparentcolor/
---
## MsoFormatPicture.TransparentColor property

Gets and sets the transparent color of the picture.

```csharp
public CellsColor TransparentColor { get; set; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(Color.White,shapes[0].FormatPicture.TransparentColor.Color);
[Test]
        public void Property_TransparentColor()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CellsJava42980.XLSX");
            Picture picture = workbook.Worksheets[0].Pictures[3];
            //workbook.Save(dir + "dest.xlsx");
            Workbook w = new Workbook();
            ShapeCollection shapes = w.Worksheets[0].Shapes;
            shapes.AddCopy(picture, 0, 0, 0, 0);
            w.Save(Constants.destPath + "CellsJava42980.xlsx");
            AssertHelper.AreEqual(Color.White,shapes[0].FormatPicture.TransparentColor.Color);
           

        }
```

### See Also

* class [CellsColor](../../../aspose.cells/cellscolor/)
* class [MsoFormatPicture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


