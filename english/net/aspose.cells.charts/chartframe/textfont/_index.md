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
// Called: Assert.AreEqual(workbook.Worksheets[0].Charts[0].Title.TextFont.Name,
// Mo Shujun Issue
public void ChartFrame_Property_TextFont()
{
    Console.WriteLine("ChartFrame_Property_TextFont()");
    string infn = path + @"ChartTitleFont\test.xlsx";
    string outfn = Constants.destPath + @"ChartTitleFont.xlsx";

    Workbook workbook = new Workbook(infn);
    Assert.AreEqual(workbook.Worksheets[0].Charts[0].Title.TextFont.Name,
        workbook.Worksheets[1].Charts[0].Title.TextFont.Name);
    workbook.Save(outfn);
}
```

### See Also

* class [Font](../../../aspose.cells/font/)
* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


