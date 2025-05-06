---
title: GroupShape.GetGroupedShapes
second_title: Aspose.Cells for .NET API Reference
description: GroupShape method. Gets the shapes grouped by this shape
type: docs
url: /net/aspose.cells.drawing/groupshape/getgroupedshapes/
---
## GroupShape.GetGroupedShapes method

Gets the shapes grouped by this shape.

```csharp
public Shape[] GetGroupedShapes()
```

### Examples

```csharp
// Called: foreach (Shape smartart in shape.GetResultOfSmartArt().GetGroupedShapes())
[Test]
        public void Method_GetGroupedShapes()
        {
            Workbook book = new Workbook(Constants.sourcePath + &quot;CellsNet46261.xlsx&quot;);
            foreach (Worksheet worksheet in book.Worksheets)
            {
                foreach (Shape shape in worksheet.Shapes)
                {
                    shape.AlternativeText = &quot;ReplacedAlternativeText&quot;; // This works fine just as the normal Shape objects do. 
                    if (shape.IsSmartArt)
                    {
                        foreach (Shape smartart in shape.GetResultOfSmartArt().GetGroupedShapes())
                        {
                            smartart.Text = &quot;ReplacedText&quot;; // This doesn&apos;t update the text in Workbook which I save to the another file. 
                        }
                    }
                }
            }
            OoxmlSaveOptions saveOptions = new OoxmlSaveOptions();
            saveOptions.UpdateSmartArt = true;
            book.Save(Constants.destPath + &quot;CellsNet46261.xlsx&quot;, saveOptions);
            book = new Workbook(Constants.destPath + &quot;CellsNet46261.xlsx&quot;);
            foreach (Worksheet worksheet in book.Worksheets)
            {
                foreach (Shape shape in worksheet.Shapes)
                {
                    Assert.AreEqual(shape.AlternativeText, &quot;ReplacedAlternativeText&quot;); // This works fine just as the normal Shape objects do. 
                    if (shape.IsSmartArt)
                    {
                        foreach (Shape smartart in shape.GetResultOfSmartArt().GetGroupedShapes())
                        {
                            Assert.AreEqual(smartart.Text, &quot;ReplacedText&quot;); // This doesn&apos;t update the text in Workbook which I save to the another file. 
                        }
                    }
                }
            }
        }
```

### See Also

* class [Shape](../../shape/)
* class [GroupShape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


