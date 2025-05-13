---
title: ChartFrame.Font
second_title: Aspose.Cells for .NET API Reference
description: ChartFrame property. Gets a Font object of the specified ChartFrame object
type: docs
url: /net/aspose.cells.charts/chartframe/font/
---
## ChartFrame.Font property

Gets a `Font` object of the specified ChartFrame object.

```csharp
public virtual Font Font { get; }
```

### Examples

```csharp
// Called: TextCapsType _type = chart.Title.Font.CapsType; //old:all. new:none.
public void ChartFrame_Property_Font()
{
    Workbook book = new Workbook(Constants.sourcePath + "example.xlsx");
    Chart chart = book.Worksheets[0].Charts[0];
    TextCapsType _type = chart.Title.Font.CapsType; //old:all. new:none.
    Assert.AreEqual(_type, TextCapsType.None);
}
```

### See Also

* class [Font](../../../aspose.cells/font/)
* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


