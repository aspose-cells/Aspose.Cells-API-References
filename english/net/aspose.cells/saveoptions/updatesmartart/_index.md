---
title: SaveOptions.UpdateSmartArt
second_title: Aspose.Cells for .NET API Reference
description: SaveOptions property. Indicates whether updating smart art setting. The default value is false
type: docs
url: /net/aspose.cells/saveoptions/updatesmartart/
---
## SaveOptions.UpdateSmartArt property

Indicates whether updating smart art setting. The default value is false.

```csharp
public bool UpdateSmartArt { get; set; }
```

### Remarks

Only effects after calling Shape.GetResultOfSmartArt() method and the cached shapes exist in the template file.

### Examples

```csharp
// Called: saveOptions.UpdateSmartArt = true;
[Test]
        public void Property_UpdateSmartArt()
        {
            Workbook book = new Workbook(Constants.sourcePath + "CellsNet46261.xlsx");
            foreach (Worksheet worksheet in book.Worksheets)
            {
                foreach (Shape shape in worksheet.Shapes)
                {
                    shape.AlternativeText = "ReplacedAlternativeText"; // This works fine just as the normal Shape objects do. 
                    if (shape.IsSmartArt)
                    {
                        foreach (Shape smartart in shape.GetResultOfSmartArt().GetGroupedShapes())
                        {
                            smartart.Text = "ReplacedText"; // This doesn't update the text in Workbook which I save to the another file. 
                        }
                    }
                }
            }
            OoxmlSaveOptions saveOptions = new OoxmlSaveOptions();
            saveOptions.UpdateSmartArt = true;
            book.Save(Constants.destPath + "CellsNet46261.xlsx", saveOptions);
            book = new Workbook(Constants.destPath + "CellsNet46261.xlsx");
            foreach (Worksheet worksheet in book.Worksheets)
            {
                foreach (Shape shape in worksheet.Shapes)
                {
                    Assert.AreEqual(shape.AlternativeText, "ReplacedAlternativeText"); // This works fine just as the normal Shape objects do. 
                    if (shape.IsSmartArt)
                    {
                        foreach (Shape smartart in shape.GetResultOfSmartArt().GetGroupedShapes())
                        {
                            Assert.AreEqual(smartart.Text, "ReplacedText"); // This doesn't update the text in Workbook which I save to the another file. 
                        }
                    }
                }
            }
        }
```

### See Also

* class [SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


