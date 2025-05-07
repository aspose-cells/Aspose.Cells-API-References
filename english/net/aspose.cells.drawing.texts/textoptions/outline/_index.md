---
title: TextOptions.Outline
second_title: Aspose.Cells for .NET API Reference
description: TextOptions property. Represents the outline format of the text
type: docs
url: /net/aspose.cells.drawing.texts/textoptions/outline/
---
## TextOptions.Outline property

Represents the outline format of the text.

```csharp
public LineFormat Outline { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(Math.Round(shape.TextOptions.Outline.Weight,2), 2.48);
[Test]
        public void Property_Outline()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CELLSJAVA42085.xlsx");
            Shape shape = workbook.Worksheets[0].Shapes[0];
            shape.Text = ("NEW TEXT");
            workbook.Save(Constants.destPath + "dest.xlsx");
            workbook = new Workbook(Constants.destPath + "dest.xlsx");
            shape = workbook.Worksheets[0].Shapes[0];
            Assert.AreEqual(Math.Round(shape.TextOptions.Outline.Weight,2), 2.48);
        }
```

### See Also

* class [LineFormat](../../../aspose.cells.drawing/lineformat/)
* class [TextOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


