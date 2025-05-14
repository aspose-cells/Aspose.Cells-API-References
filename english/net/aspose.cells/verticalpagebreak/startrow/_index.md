---
title: VerticalPageBreak.StartRow
second_title: Aspose.Cells for .NET API Reference
description: VerticalPageBreak property. Gets the start row index of the vertical page break
type: docs
url: /net/aspose.cells/verticalpagebreak/startrow/
---
## VerticalPageBreak.StartRow property

Gets the start row index of the vertical page break.

```csharp
public int StartRow { get; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(vpagebreakSrc.StartRow, vpagebreakDest.StartRow, info + ".StartRow");
public static void VerticalPageBreak_Property_StartRow(VerticalPageBreak vpagebreakSrc, VerticalPageBreak vpagebreakDest, string info)
        {
            if (AssertHelper.checkNull(vpagebreakSrc, vpagebreakDest, info))
            {
                return;
            }
            AssertHelper.AreEqual(vpagebreakSrc.StartRow, vpagebreakDest.StartRow, info + ".StartRow");
            AssertHelper.AreEqual(vpagebreakSrc.EndRow, vpagebreakDest.EndRow, info + ".EndRow");
            AssertHelper.AreEqual(vpagebreakSrc.Column, vpagebreakDest.Column, info + ".Column");
        }
```

### See Also

* class [VerticalPageBreak](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


