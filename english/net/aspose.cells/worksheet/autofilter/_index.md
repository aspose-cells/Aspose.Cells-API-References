---
title: Worksheet.AutoFilter
second_title: Aspose.Cells for .NET API Reference
description: Worksheet property. Represents auto filter for the specified worksheet
type: docs
url: /net/aspose.cells/worksheet/autofilter/
---
## Worksheet.AutoFilter property

Represents auto filter for the specified worksheet.

```csharp
public AutoFilter AutoFilter { get; }
```

### Examples

```csharp
// Called: AutoFilter af = sheet.AutoFilter;
[Test]
        public void Property_AutoFilter()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;
            cells[1, 0].PutValue(&quot;US&quot;);
            cells[2, 0].PutValue(&quot;UK&quot;);
            cells[3, 0].PutValue(&quot;India&quot;);
            cells[4, 0].PutValue(&quot;UK&quot;);
            cells[5, 0].PutValue(&quot;India&quot;);
            cells[6, 0].PutValue(&quot;US&quot;);
            for (int i = 1; i &lt; 10; i++)
            {
                cells[i, 1].PutValue(i);
            }
            AutoFilter af = sheet.AutoFilter;
            af.Range = &quot;A1:A1&quot;;
            af.Filter(0, &quot;India&quot;);
            af.Refresh();
            for (int i = 1; i &lt; 10; i++)
            {
                Assert.AreEqual(i != 3 &amp;&amp; i != 5, cells.IsRowHidden(i), &quot;Row-&quot; + i + &quot;.Hidden&quot;);
            }
        }
```

### See Also

* class [AutoFilter](../../autofilter/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


