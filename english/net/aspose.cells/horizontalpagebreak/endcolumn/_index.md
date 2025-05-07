---
title: HorizontalPageBreak.EndColumn
second_title: Aspose.Cells for .NET API Reference
description: HorizontalPageBreak property. Gets the end column index of this horizontal page break
type: docs
url: /net/aspose.cells/horizontalpagebreak/endcolumn/
---
## HorizontalPageBreak.EndColumn property

Gets the end column index of this horizontal page break.

```csharp
public int EndColumn { get; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(255, hpagebreak.EndColumn, "hpagebreak.EndColumn");
[Test]
        public void Property_EndColumn()
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

* class [HorizontalPageBreak](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


