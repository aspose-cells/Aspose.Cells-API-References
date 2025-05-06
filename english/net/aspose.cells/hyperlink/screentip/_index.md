---
title: Hyperlink.ScreenTip
second_title: Aspose.Cells for .NET API Reference
description: Hyperlink property. Returns or sets the ScreenTip text for the specified hyperlink
type: docs
url: /net/aspose.cells/hyperlink/screentip/
---
## Hyperlink.ScreenTip property

Returns or sets the ScreenTip text for the specified hyperlink.

```csharp
public string ScreenTip { get; set; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(hlinkSrc.ScreenTip, hlinkDest.ScreenTip, info + &amp;quot;.ScreenTip&amp;quot;);
public static void Property_ScreenTip(Hyperlink hlinkSrc, Hyperlink hlinkDest, string info)
        {
            if (AssertHelper.checkNull(hlinkSrc, hlinkDest, info))
            {
                return;
            }
            AssertHelper.AreEqual(hlinkSrc.Address, hlinkDest.Address, info + &quot;.Address&quot;);
            CellAreaTest.Property_ScreenTip(hlinkSrc.Area, hlinkDest.Area, info + &quot;.Area&quot;);
            AssertHelper.AreEqual(hlinkSrc.ScreenTip, hlinkDest.ScreenTip, info + &quot;.ScreenTip&quot;);
            AssertHelper.AreEqual(hlinkSrc.TextToDisplay, hlinkDest.TextToDisplay, info + &quot;.TextToDisplay&quot;);
        }
```

### See Also

* class [Hyperlink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


