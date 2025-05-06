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
// Called: AssertHelper.AreEqual(vpagebreakSrc.Column, vpagebreakDest.Column, info + &amp;quot;.Column&amp;quot;);
public static void Property_Column(VerticalPageBreak vpagebreakSrc, VerticalPageBreak vpagebreakDest, string info)
        {
            if (AssertHelper.checkNull(vpagebreakSrc, vpagebreakDest, info))
            {
                return;
            }
            AssertHelper.AreEqual(vpagebreakSrc.StartRow, vpagebreakDest.StartRow, info + &quot;.StartRow&quot;);
            AssertHelper.AreEqual(vpagebreakSrc.EndRow, vpagebreakDest.EndRow, info + &quot;.EndRow&quot;);
            AssertHelper.AreEqual(vpagebreakSrc.Column, vpagebreakDest.Column, info + &quot;.Column&quot;);
        }
```

### See Also

* class [VerticalPageBreak](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


