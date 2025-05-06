---
title: PatternFill.Pattern
second_title: Aspose.Cells for .NET API Reference
description: PatternFill property. Gets or sets the fill pattern type
type: docs
url: /net/aspose.cells.drawing/patternfill/pattern/
---
## PatternFill.Pattern property

Gets or sets the fill pattern type

```csharp
public FillPattern Pattern { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(FillPattern.LightUpwardDiagonal, shape.Fill.PatternFill.Pattern);
[Test]
        public void Property_Pattern()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CELLSJAVA45132.xls&quot;);
            Shape shape = workbook.Worksheets[&quot;Notes (2)&quot;].Shapes[0];
            Assert.AreEqual(FillPattern.LightUpwardDiagonal, shape.Fill.PatternFill.Pattern);
        }
```

### See Also

* enum [FillPattern](../../fillpattern/)
* class [PatternFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


