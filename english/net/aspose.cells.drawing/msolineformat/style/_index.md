---
title: MsoLineFormat.Style
second_title: Aspose.Cells for .NET API Reference
description: MsoLineFormat property. Returns a Style object that represents the style of the specified range
type: docs
url: /net/aspose.cells.drawing/msolineformat/style/
---
## MsoLineFormat.Style property

Returns a Style object that represents the style of the specified range.

```csharp
public MsoLineStyle Style { get; set; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(msolformatSrc.Style, msolformatDest.Style, info + &amp;quot;.Style&amp;quot;);
public static void Property_Style(MsoLineFormat msolformatSrc, MsoLineFormat msolformatDest, string info)
        {
            if (AssertHelper.checkNull(msolformatSrc, msolformatDest, info))
            {
                return;
            }
            AssertHelper.AreEqual(msolformatSrc.IsVisible, msolformatDest.IsVisible, info + &quot;.IsVisible&quot;);
            if (msolformatSrc.IsVisible &amp;&amp; msolformatDest.IsVisible)
            {
                AssertHelper.Property_Style(msolformatSrc.BackColor, msolformatDest.BackColor, info + &quot;.BackColor&quot;);
                AssertHelper.Property_Style(msolformatSrc.ForeColor, msolformatDest.ForeColor, info + &quot;.ForeColor&quot;);
                AssertHelper.AreEqual(msolformatSrc.DashStyle, msolformatDest.DashStyle, info + &quot;.DashStyle&quot;);
                AssertHelper.AreEqual(msolformatSrc.Style, msolformatDest.Style, info + &quot;.Style&quot;);
                AssertHelper.AreEqual(msolformatSrc.Transparency, msolformatDest.Transparency, delta, info + &quot;.Transparency&quot;);
                AssertHelper.AreEqual(msolformatSrc.Weight, msolformatDest.Weight, delta, info + &quot;.Weight&quot;);
            }
           

        }
```

### See Also

* enum [MsoLineStyle](../../msolinestyle/)
* class [MsoLineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


