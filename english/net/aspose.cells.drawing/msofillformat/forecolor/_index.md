---
title: MsoFillFormat.ForeColor
second_title: Aspose.Cells for .NET API Reference
description: MsoFillFormat property. Gets and sets the fill fore color
type: docs
url: /net/aspose.cells.drawing/msofillformat/forecolor/
---
## MsoFillFormat.ForeColor property

Gets and sets the fill fore color.

```csharp
public Color ForeColor { get; set; }
```

### Examples

```csharp
// Called: AssertHelper.equals(msofformatSrc.ForeColor, msofformatDest.ForeColor, info + &amp;quot;.ForeColor&amp;quot;);
public static void Property_ForeColor(MsoFillFormat msofformatSrc, MsoFillFormat msofformatDest, string info)
        {
            if (AssertHelper.checkNull(msofformatSrc, msofformatDest, info))
            {
                return;
            }
            AssertHelper.AreEqual(msofformatSrc.IsVisible, msofformatDest.IsVisible, info + &quot;.IsVisible&quot;);
            if (msofformatSrc.IsVisible)
            {                
                AssertHelper.Property_ForeColor(msofformatSrc.ForeColor, msofformatDest.ForeColor, info + &quot;.ForeColor&quot;);
                AssertHelper.Property_ForeColor(msofformatSrc.BackColor, msofformatDest.BackColor, info + &quot;.BackColor&quot;);
                AssertHelper.AreEqual(msofformatSrc.Transparency, msofformatDest.Transparency, 0.01, info + &quot;.Transparency&quot;);
                if(msofformatDest.ImageData != null)
                    AssertHelper.Property_ForeColor(msofformatSrc.ImageData, msofformatDest.ImageData, info + &quot;.ImageData&quot;);
                AssertHelper.AreEqual(msofformatSrc.Texture, msofformatDest.Texture, info + &quot;.Texture&quot;);
            }
        }
```

### See Also

* class [MsoFillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


