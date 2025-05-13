---
title: VerticalPageBreak.Column
second_title: Aspose.Cells for .NET API Reference
description: VerticalPageBreak property. Gets the column index of the vertical page break
type: docs
url: /net/aspose.cells/verticalpagebreak/column/
---
## VerticalPageBreak.Column property

Gets the column index of the vertical page break.

```csharp
public int Column { get; }
```

### Examples

```csharp
// Called: if (vpagebreak.Column == 4 || vpagebreak.Column == 8)
public void VerticalPageBreak_Property_Column()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "Worksheet\\PageBreak.xls");
    Worksheet worksheet = workbook.Worksheets[0];
    HorizontalPageBreakCollection hpagebreaks = worksheet.HorizontalPageBreaks;
    AssertHelper.AreEqual(3, hpagebreaks.Count, "hpagebreaks.Count");
    HorizontalPageBreak hpagebreak;
    for (int i = 0; i < hpagebreaks.Count; i++)
    {
        hpagebreak = hpagebreaks[i];
        if (hpagebreak.Row == 1 || hpagebreak.Row == 6 || hpagebreak.Row == 11)
        {
            AssertHelper.AreEqual(0, hpagebreak.StartColumn, "hpagebreak.StartColumn");
            AssertHelper.AreEqual(255, hpagebreak.EndColumn, "hpagebreak.EndColumn");
            continue;
        }
        AssertHelper.Fail("Fail");
    }
    VerticalPageBreakCollection vpagebreaks = worksheet.VerticalPageBreaks;
    AssertHelper.AreEqual(2, vpagebreaks.Count, "vpagebreaks.Count");
    VerticalPageBreak vpagebreak;
    for (int i = 0; i < vpagebreaks.Count; i++)
    {
        vpagebreak = vpagebreaks[i];
        if (vpagebreak.Column == 4 || vpagebreak.Column == 8)
        {
            AssertHelper.AreEqual(0, vpagebreak.StartRow, "vpagebreak.StartRow");
            AssertHelper.AreEqual(65535, vpagebreak.EndRow, "vpagebreak.EndRow");
            continue;
        }
        AssertHelper.Fail("Fail");
    }

}
```

### See Also

* class [VerticalPageBreak](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


