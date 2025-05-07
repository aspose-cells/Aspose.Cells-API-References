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
// Called: AssertHelper.equals(msofformatSrc.ForeColor, msofformatDest.ForeColor, info + ".ForeColor");
public static void Property_ForeColor(MsoFillFormat msofformatSrc, MsoFillFormat msofformatDest, string info)
        {
            if (AssertHelper.checkNull(msofformatSrc, msofformatDest, info))
            {
                return;
            }
            AssertHelper.AreEqual(msofformatSrc.IsVisible, msofformatDest.IsVisible, info + ".IsVisible");
            if (msofformatSrc.IsVisible)
            {                
                AssertHelper.Property_ForeColor(msofformatSrc.ForeColor, msofformatDest.ForeColor, info + ".ForeColor");
                AssertHelper.Property_ForeColor(msofformatSrc.BackColor, msofformatDest.BackColor, info + ".BackColor");
                AssertHelper.AreEqual(msofformatSrc.Transparency, msofformatDest.Transparency, 0.01, info + ".Transparency");
                if(msofformatDest.ImageData != null)
                    AssertHelper.Property_ForeColor(msofformatSrc.ImageData, msofformatDest.ImageData, info + ".ImageData");
                AssertHelper.AreEqual(msofformatSrc.Texture, msofformatDest.Texture, info + ".Texture");
            }
        }
```

### See Also

* class [MsoFillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


