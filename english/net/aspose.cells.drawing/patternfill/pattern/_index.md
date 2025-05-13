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
// Called: Assert.AreEqual(chart.NSeries[3].Area.FillFormat.PatternFill.Pattern, FillPattern.WideDownwardDiagonal);
public void PatternFill_Property_Pattern()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xls");
    Chart chart = workbook.Worksheets[0].Charts[6];
    Assert.AreEqual(chart.Worksheet.Index, 0);//CELLSJAVA-41019
    Assert.AreEqual(chart.NSeries[3].Area.FillFormat.FillType, FillType.Pattern);
    Assert.AreEqual(chart.NSeries[3].Area.FillFormat.PatternFill.Pattern, FillPattern.WideDownwardDiagonal);
}
```

### See Also

* enum [FillPattern](../../fillpattern/)
* class [PatternFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


