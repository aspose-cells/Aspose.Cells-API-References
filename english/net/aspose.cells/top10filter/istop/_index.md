---
title: Top10Filter.IsTop
second_title: Aspose.Cells for .NET API Reference
description: Top10Filter property. Indicates whether its top filter
type: docs
url: /net/aspose.cells/top10filter/istop/
---
## Top10Filter.IsTop property

Indicates whether it's top filter.

```csharp
public bool IsTop { get; set; }
```

### Examples

```csharp
// Called: Assert.IsTrue(f.IsTop);
[Test]
        public void Property_IsTop()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;AutoFilter/N46267.xlsx&quot;);
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.AutoFilter.Range = &quot;B6:K10&quot;;
            worksheet.AutoFilter.FilterTop10(5, true, false, 5);
            Top10Filter f = worksheet.AutoFilter.FilterColumns[5].Filter as Top10Filter;
            Assert.IsNotNull(f);
            Assert.IsTrue(f.IsTop);
            Assert.IsFalse(f.IsPercent);
            worksheet.AutoFilter.Refresh();
            Cells cells = worksheet.Cells;
            for (int i = 6; i &lt; 30; i++)
            {
                Assert.AreEqual(i != 7 &amp;&amp; i != 8 &amp;&amp; i != 11 &amp;&amp; i != 12 &amp;&amp; i != 16,
                    cells.IsRowHidden(i), &quot;Row(0 based).Hidden-&quot; + i);
            }
        }
```

### See Also

* class [Top10Filter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


