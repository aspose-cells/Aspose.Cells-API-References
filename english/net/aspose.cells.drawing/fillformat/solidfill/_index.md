---
title: FillFormat.SolidFill
second_title: Aspose.Cells for .NET API Reference
description: FillFormat property. Gets SolidFill object
type: docs
url: /net/aspose.cells.drawing/fillformat/solidfill/
---
## FillFormat.SolidFill property

Gets `SolidFill` object.

```csharp
public SolidFill SolidFill { get; }
```

### Examples

```csharp
// Called: chart.NSeries[0].Area.FillFormat.SolidFill.CellsColor = cc;
[Test]
        public void Property_SolidFill()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CellsNet40829.xlsx&quot;);
            Chart chart = workbook.Worksheets[0].Charts[0];
            CellsColor cc = chart.NSeries[0].Area.FillFormat.SolidFill.CellsColor;
            cc.ThemeColor = new ThemeColor(ThemeColorType.Accent6, 0.6);
            chart.NSeries[0].Area.FillFormat.SolidFill.CellsColor = cc;
            workbook.Save(Constants.destPath + &quot;CellsNet40829.xlsx&quot;);
            workbook = new Workbook(Constants.destPath + &quot;CellsNet40829.xlsx&quot;);
            Assert.AreEqual(workbook.Worksheets[0].Charts[0].NSeries[0].Area.FillFormat.SolidFill.Color.ToArgb() &amp; 0xFFFFFF, Color.FromArgb(252, 213, 181).ToArgb() &amp; 0xFFFFFF);
            Assert.AreEqual(workbook.Worksheets[0].Charts[0].NSeries[0].Area.FillFormat.SolidFill.CellsColor.ThemeColor.Tint, 0.6);
        }
```

### See Also

* class [SolidFill](../../solidfill/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


