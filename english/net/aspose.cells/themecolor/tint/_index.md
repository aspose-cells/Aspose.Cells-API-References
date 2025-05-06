---
title: ThemeColor.Tint
second_title: Aspose.Cells for .NET API Reference
description: ThemeColor property. Gets and sets the tint value
type: docs
url: /net/aspose.cells/themecolor/tint/
---
## ThemeColor.Tint property

Gets and sets the tint value.

```csharp
public double Tint { get; set; }
```

### Remarks

The tint value is stored as a double from -1.0 .. 1.0, where -1.0 means 100% darken and 1.0 means 100% lighten. Also, 0.0 means no change.

### Examples

```csharp
// Called: Assert.AreEqual(workbook.Worksheets[0].Charts[0].NSeries[0].Area.FillFormat.SolidFill.CellsColor.ThemeColor.Tint, 0.6);
[Test]
        public void Property_Tint()
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

* class [ThemeColor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


