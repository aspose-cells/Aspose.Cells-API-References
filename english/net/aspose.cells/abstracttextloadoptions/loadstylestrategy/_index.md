---
title: AbstractTextLoadOptions.LoadStyleStrategy
second_title: Aspose.Cells for .NET API Reference
description: AbstractTextLoadOptions property. Indicates the strategy to apply style for parsed values when converting string value to number or datetime
type: docs
url: /net/aspose.cells/abstracttextloadoptions/loadstylestrategy/
---
## AbstractTextLoadOptions.LoadStyleStrategy property

Indicates the strategy to apply style for parsed values when converting string value to number or datetime.

```csharp
public TxtLoadStyleStrategy LoadStyleStrategy { get; set; }
```

### Examples

```csharp
// Called: wb = new Workbook(Constants.sourcePath + &amp;quot;CELLSJAVA41014.csv&amp;quot;, new TxtLoadOptions() { LoadStyleStrategy = TxtLoadStyleStrategy.BuiltIn });
[Test]
        public void Property_LoadStyleStrategy()
        {
            Workbook wb = new Workbook(Constants.sourcePath + &quot;CELLSJAVA41014.csv&quot;, new TxtLoadOptions());
            Cells cells = wb.Worksheets[0].Cells;
            for (int i = cells.MaxDataRow; i &gt; -1; i--)
            {
                Style style = cells[i, 0].GetStyle();
                if (string.IsNullOrEmpty(style.Custom))
                {
                    Assert.Fail(&quot;With default load option, A&quot; + (i + 1) + &quot;&apos;s custom should not be null&quot;);
                }
            }
            wb = new Workbook(Constants.sourcePath + &quot;CELLSJAVA41014.csv&quot;, new TxtLoadOptions() { LoadStyleStrategy = TxtLoadStyleStrategy.BuiltIn });
            cells = wb.Worksheets[0].Cells;
            for (int i = cells.MaxDataRow; i &gt; -1; i--)
            {
                Style style = cells[i, 0].GetStyle();
                if (!string.IsNullOrEmpty(style.Custom))
                {
                    Assert.Fail(&quot;With option KeepExactFormat = false, A&quot; + (i + 1) + &quot;&apos;s custom is not null, in fact it should be parsed as builtin format.&quot;);
                }
                if (style.Number == 0)
                {
                    Assert.Fail(&quot;With option KeepExactFormat = false, A&quot; + (i + 1) + &quot;&apos;s number is 0, in fact it should be parsed as builtin format.&quot;);
                }
            }
        }
```

### See Also

* enum [TxtLoadStyleStrategy](../../txtloadstylestrategy/)
* class [AbstractTextLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


