---
title: HorizontalPageBreak.StartColumn
second_title: Aspose.Cells for .NET API Reference
description: HorizontalPageBreak property. Gets the start column index of this horizontal page break
type: docs
url: /net/aspose.cells/horizontalpagebreak/startcolumn/
---
## HorizontalPageBreak.StartColumn property

Gets the start column index of this horizontal page break.

```csharp
public int StartColumn { get; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(hpagebreaSrc.StartColumn, hpagebreakDest.StartColumn, info + &amp;quot;.StartColumn&amp;quot;);
public static void Property_StartColumn(HorizontalPageBreak hpagebreaSrc, HorizontalPageBreak hpagebreakDest, string info)
        {
            if (AssertHelper.checkNull(hpagebreaSrc, hpagebreakDest, info))
            {
                return;
            }
            AssertHelper.AreEqual(hpagebreaSrc.StartColumn, hpagebreakDest.StartColumn, info + &quot;.StartColumn&quot;);
            AssertHelper.AreEqual(hpagebreaSrc.EndColumn, hpagebreakDest.EndColumn, info + &quot;.EndColumn&quot;);
            AssertHelper.AreEqual(hpagebreaSrc.Row, hpagebreakDest.Row, info + &quot;.Row&quot;);
        }
```

### See Also

* class [HorizontalPageBreak](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


