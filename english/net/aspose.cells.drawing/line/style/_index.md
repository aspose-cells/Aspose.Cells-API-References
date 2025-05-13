---
title: Line.Style
second_title: Aspose.Cells for .NET API Reference
description: Line property. Represents the style of the line
type: docs
url: /net/aspose.cells.drawing/line/style/
---
## Line.Style property

Represents the style of the line.

```csharp
public LineType Style { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(p.Border.Style, Aspose.Cells.Drawing.LineType.Solid);
public void Line_Property_Style()
{
    Workbook wb = new Workbook(Constants.sourcePath + "example.xls");
    Chart c = wb.Worksheets[0].Charts[0];
    Series s = c.NSeries[0];
    ChartPoint p = s.Points[1];
    p.Border.Color = Color.Red; //it works
    p.Border.Style = Aspose.Cells.Drawing.LineType.Solid; //it does not work
    Assert.AreEqual(p.Border.Style, Aspose.Cells.Drawing.LineType.Solid);

    wb.Save(Constants.destPath + "example.xls");

}
```

### See Also

* enum [LineType](../../linetype/)
* class [Line](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


