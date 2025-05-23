---
title: MsoFormatPicture.IsGray
second_title: Aspose.Cells for .NET API Reference
description: MsoFormatPicture property. Indicates whether this picture should display in grayscale
type: docs
url: /net/aspose.cells.drawing/msoformatpicture/isgray/
---
## MsoFormatPicture.IsGray property

Indicates whether this picture should display in grayscale.

```csharp
public bool IsGray { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(shape.FormatPicture.IsGray,true);
public void MsoFormatPicture_Property_IsGray()
{
    Workbook workbook = new Workbook(Constants.sourcePath + @"example.xlsx");
    {
        int index = 0;
        using (Stream imageStream = File.OpenRead(Path.Combine(Constants.sourcePath, @"example.gif")))
        {
            Shape shape = workbook.Worksheets[0].Shapes.AddPicture(0, 0, imageStream, 100, 100);
            index = shape.ZOrderPosition;
            CellsColor cellsColor = workbook.CreateCellsColor();
            cellsColor.Color = Color.White;
            cellsColor.IsShapeColor = true;
            shape.FormatPicture.TransparentColor = cellsColor;

            shape.FormatPicture.Brightness = 90;
            shape.FormatPicture.Contrast = 90;
            shape.FormatPicture.IsGray = true;
        }
        workbook.Save(Constants.destPath + "example.xlsx");
        workbook = new Workbook(Constants.destPath + "example.xlsx");
        {
            Shape shape = workbook.Worksheets[0].Shapes[index];
            Assert.AreEqual( shape.FormatPicture.Brightness , 90);
            Assert.AreEqual(shape.FormatPicture.Contrast, 90);
            Assert.AreEqual(shape.FormatPicture.IsGray,true);
        }
        Util.SaveManCheck(workbook, "Shape", "example.xlsx");

                
    }
}
```

### See Also

* class [MsoFormatPicture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


