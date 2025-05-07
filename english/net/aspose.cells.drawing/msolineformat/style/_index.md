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
// Called: AssertHelper.AreEqual(msolformatSrc.Style, msolformatDest.Style, info + ".Style");
public static void Property_Style(MsoLineFormat msolformatSrc, MsoLineFormat msolformatDest, string info)
        {
            if (AssertHelper.checkNull(msolformatSrc, msolformatDest, info))
            {
                return;
            }
            AssertHelper.AreEqual(msolformatSrc.IsVisible, msolformatDest.IsVisible, info + ".IsVisible");
            if (msolformatSrc.IsVisible && msolformatDest.IsVisible)
            {
                AssertHelper.Property_Style(msolformatSrc.BackColor, msolformatDest.BackColor, info + ".BackColor");
                AssertHelper.Property_Style(msolformatSrc.ForeColor, msolformatDest.ForeColor, info + ".ForeColor");
                AssertHelper.AreEqual(msolformatSrc.DashStyle, msolformatDest.DashStyle, info + ".DashStyle");
                AssertHelper.AreEqual(msolformatSrc.Style, msolformatDest.Style, info + ".Style");
                AssertHelper.AreEqual(msolformatSrc.Transparency, msolformatDest.Transparency, delta, info + ".Transparency");
                AssertHelper.AreEqual(msolformatSrc.Weight, msolformatDest.Weight, delta, info + ".Weight");
            }
           

        }
```

### See Also

* enum [MsoLineStyle](../../msolinestyle/)
* class [MsoLineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


