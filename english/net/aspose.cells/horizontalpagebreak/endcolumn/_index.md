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
// Called: AssertHelper.AreEqual(hpagebreaSrc.EndColumn, hpagebreakDest.EndColumn, info + ".EndColumn");
public static void HorizontalPageBreak_Property_EndColumn(HorizontalPageBreak hpagebreaSrc, HorizontalPageBreak hpagebreakDest, string info)
        {
            if (AssertHelper.checkNull(hpagebreaSrc, hpagebreakDest, info))
            {
                return;
            }
            AssertHelper.AreEqual(hpagebreaSrc.StartColumn, hpagebreakDest.StartColumn, info + ".StartColumn");
            AssertHelper.AreEqual(hpagebreaSrc.EndColumn, hpagebreakDest.EndColumn, info + ".EndColumn");
            AssertHelper.AreEqual(hpagebreaSrc.Row, hpagebreakDest.Row, info + ".Row");
        }
```

### See Also

* class [HorizontalPageBreak](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


