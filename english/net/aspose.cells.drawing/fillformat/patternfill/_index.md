---
title: FillFormat.PatternFill
second_title: Aspose.Cells for .NET API Reference
description: FillFormat property. Gets PatternFill object
type: docs
url: /net/aspose.cells.drawing/fillformat/patternfill/
---
## FillFormat.PatternFill property

Gets `PatternFill` object.

```csharp
public PatternFill PatternFill { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(FillPattern.LightUpwardDiagonal, shape.Fill.PatternFill.Pattern);
[Test]
        public void Property_PatternFill()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CELLSJAVA45132.xls");
            Shape shape = workbook.Worksheets["Notes (2)"].Shapes[0];
            Assert.AreEqual(FillPattern.LightUpwardDiagonal, shape.Fill.PatternFill.Pattern);
        }
```

### See Also

* class [PatternFill](../../patternfill/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


