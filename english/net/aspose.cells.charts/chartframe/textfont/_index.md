---
title: ChartFrame.TextFont
second_title: Aspose.Cells for .NET API Reference
description: ChartFrame property. Gets a Font object of the specified ChartFrame object
type: docs
url: /net/aspose.cells.charts/chartframe/textfont/
---
## ChartFrame.TextFont property

Gets a [`Font`](../font/) object of the specified ChartFrame object.

```csharp
[Obsolete("Use ChartFrame.Font property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public virtual Font TextFont { get; }
```

### Remarks

NOTE: This member is now obsolete. Instead, please use ChartFrame.Font property. This property will be removed 12 months later since JANUARY 2012. Aspose apologizes for any inconvenience you may have experienced.

### Examples

```csharp
// Called: Assert.AreEqual(chart.NSeries[2].Points[4].DataLabels.TextFont.Color.ToArgb() & 0xFFFFFF,
[Test]
        public void Property_TextFont()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CellsNet19911.xls");
            Workbook b = new Workbook(Constants.sourcePath + "CellsNet19911.xls");
            workbook.Combine(b);
            Chart chart = workbook.Worksheets[1].Charts[0];
            Assert.AreEqual(chart.NSeries[2].Points[4].DataLabels.TextFont.Color.ToArgb() & 0xFFFFFF,
                0xFF00FF);
            workbook.Save(Constants.destPath + "CellsNet19911.xls");

        }
```

### See Also

* class [Font](../../../aspose.cells/font/)
* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


