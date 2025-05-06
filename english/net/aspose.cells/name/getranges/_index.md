---
title: Name.GetRanges
second_title: Aspose.Cells for .NET API Reference
description: Name method. Gets all ranges referred by this name
type: docs
url: /net/aspose.cells/name/getranges/
---
## GetRanges() {#getranges}

Gets all ranges referred by this name.

```csharp
public Range[] GetRanges()
```

### Return Value

All ranges.

### Examples

```csharp
// Called: Aspose.Cells.Range[] rs = name.GetRanges();
[Test]
        public void Method_GetRanges()
        {
            Workbook wb = new Workbook(Constants.sourcePath + &quot;J42118_815971.xlsx&quot;);
            NameCollection names = wb.Worksheets.Names;
            StringBuilder sb = new StringBuilder();
            for (int i = names.Count - 1; i &gt; -1; i--)
            {
                Name name = names[i];

                // determine the Refers To Type (reference|formula)
                Aspose.Cells.Range[] rs = name.GetRanges();
                if (rs != null &amp;&amp; rs.Length &gt; 0 &amp;&amp; rs[0] == null)
                {
                    // ERROR: name.getRanges().length is &gt; 0 - BUT name.getRanges()[0] is null
                    sb.Append(&quot;\nERROR! Invalid Name.GetRanges() for &quot; + name.FullText
                              + (name.SheetIndex == 0 ? &quot;: GLOBAL&quot; : &quot;: LOCAL&quot;)
                              + &quot;, Visible=&quot; + name.IsVisible + &quot;, RefersTo=&quot; + name.RefersTo);
                }
            }
            if (sb.Length &gt; 0)
            {
                Assert.Fail(sb.ToString());
            }
            Cell cell = wb.Worksheets[0].Cells[10, 0];
            cell.Formula = &quot;=_HC1&quot;;
            wb.CalculateFormula(false);
            Assert.AreEqual(&quot;#NAME?&quot;, cell.Value, &quot;SelfReference Name&apos;s calculated result&quot;);
        }
```

### See Also

* class [Range](../../range/)
* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetRanges(bool) {#getranges_1}

Gets all ranges referred by this name.

```csharp
public Range[] GetRanges(bool recalculate)
```

| Parameter | Type | Description |
| --- | --- | --- |
| recalculate | Boolean | whether recalculate it if this name has been calculated before this invocation. |

### Return Value

All ranges.

### Examples

```csharp
// Called: Aspose.Cells.Range[] ranges = recalculate ? name.GetRanges() : name.GetRanges(false);
private static void Method_Boolean_(string msg, NameCollection names, bool recalculate)
        {
            int rc = 0;
            int nc = 0;
            foreach (Name name in names)
            {
                Aspose.Cells.Range[] ranges = recalculate ? name.GetRanges() : name.GetRanges(false);
                if (ranges != null)
                {
                    rc++;
                }
                else
                {
                    nc++;
                }
            }
            if (msg != null)
            {
                Console.WriteLine(msg + rc + &quot;, &quot; + nc);
            }
        }
```

### See Also

* class [Range](../../range/)
* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


