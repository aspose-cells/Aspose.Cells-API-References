---
title: HorizontalPageBreak.Row
second_title: Aspose.Cells for .NET API Reference
description: HorizontalPageBreak property. Gets the zero based row index
type: docs
url: /net/aspose.cells/horizontalpagebreak/row/
---
## HorizontalPageBreak.Row property

Gets the zero based row index.

```csharp
public int Row { get; }
```

### Examples

```csharp
// Called: if (hpagebreak.Row == 1 || hpagebreak.Row == 6 || hpagebreak.Row == 11)
[Test]
        public void Property_Row()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;Worksheet\\PageBreak.xls&quot;);
            Worksheet worksheet = workbook.Worksheets[0];
            HorizontalPageBreakCollection hpagebreaks = worksheet.HorizontalPageBreaks;
            AssertHelper.AreEqual(3, hpagebreaks.Count, &quot;hpagebreaks.Count&quot;);
            HorizontalPageBreak hpagebreak;
            for (int i = 0; i &lt; hpagebreaks.Count; i++)
            {
                hpagebreak = hpagebreaks[i];
                if (hpagebreak.Row == 1 || hpagebreak.Row == 6 || hpagebreak.Row == 11)
                {
                    AssertHelper.AreEqual(0, hpagebreak.StartColumn, &quot;hpagebreak.StartColumn&quot;);
                    AssertHelper.AreEqual(255, hpagebreak.EndColumn, &quot;hpagebreak.EndColumn&quot;);
                    continue;
                }
                AssertHelper.Fail(&quot;Fail&quot;);
            }
            VerticalPageBreakCollection vpagebreaks = worksheet.VerticalPageBreaks;
            AssertHelper.AreEqual(2, vpagebreaks.Count, &quot;vpagebreaks.Count&quot;);
            VerticalPageBreak vpagebreak;
            for (int i = 0; i &lt; vpagebreaks.Count; i++)
            {
                vpagebreak = vpagebreaks[i];
                if (vpagebreak.Column == 4 || vpagebreak.Column == 8)
                {
                    AssertHelper.AreEqual(0, vpagebreak.StartRow, &quot;vpagebreak.StartRow&quot;);
                    AssertHelper.AreEqual(65535, vpagebreak.EndRow, &quot;vpagebreak.EndRow&quot;);
                    continue;
                }
                AssertHelper.Fail(&quot;Fail&quot;);
            }

        }
```

### See Also

* class [HorizontalPageBreak](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


