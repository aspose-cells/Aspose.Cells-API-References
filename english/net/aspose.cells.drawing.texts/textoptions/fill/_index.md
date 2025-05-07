---
title: TextOptions.Fill
second_title: Aspose.Cells for .NET API Reference
description: TextOptions property. Represents the fill format of the text
type: docs
url: /net/aspose.cells.drawing.texts/textoptions/fill/
---
## TextOptions.Fill property

Represents the fill format of the text.

```csharp
public FillFormat Fill { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(font.Fill.SolidFill.Transparency,0.5);
[Test]
        public void Property_Fill()
        {
            Aspose.Cells.Workbook workbook = new Aspose.Cells.Workbook(Constants.sourcePath + "CELLSJAVA41739.xls");
            //  Console.WriteLine(workbook.Worksheets[0].Shapes[0].ShadowEffect.Blur);
            TextOptions font = workbook.Worksheets[0].Shapes[0].TextBody[2].TextOptions;
            Assert.AreEqual(font.Fill.SolidFill.Transparency,0.5);
            workbook.Save(Constants.destPath + "CELLSJAVA41739.xlsx");
            
        }
```

### See Also

* class [FillFormat](../../../aspose.cells.drawing/fillformat/)
* class [TextOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


