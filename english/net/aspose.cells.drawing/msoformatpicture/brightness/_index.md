---
title: MsoFormatPicture.Brightness
second_title: Aspose.Cells for .NET API Reference
description: MsoFormatPicture property. Represents the brightness modification for the picture in unit of percentage
type: docs
url: /net/aspose.cells.drawing/msoformatpicture/brightness/
---
## MsoFormatPicture.Brightness property

Represents the brightness modification for the picture in unit of percentage.

```csharp
public double Brightness { get; set; }
```

### Remarks

It is between -100% and 100%. It works same as Excel 2007 or above version.

### Examples

```csharp
// Called: Assert.AreEqual( shape.FormatPicture.Brightness , 90);
[Test]
        public void Property_Brightness()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + @&quot;CELLSNET45173.xlsx&quot;);
            {
                int index = 0;
                using (Stream imageStream = File.OpenRead(Path.Combine(Constants.sourcePath, @&quot;CELLSNET45173.gif&quot;)))
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
                workbook.Save(Constants.destPath + &quot;CELLSNET45175.xlsx&quot;);
                workbook = new Workbook(Constants.destPath + &quot;CELLSNET45175.xlsx&quot;);
                {
                    Shape shape = workbook.Worksheets[0].Shapes[index];
                    Assert.AreEqual( shape.FormatPicture.Brightness , 90);
                    Assert.AreEqual(shape.FormatPicture.Contrast, 90);
                    Assert.AreEqual(shape.FormatPicture.IsGray,true);
                }
                Util.SaveManCheck(workbook, &quot;Shape&quot;, &quot;CELLSNET45175.xlsx&quot;);

                
            }
        }
```

### See Also

* class [MsoFormatPicture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


