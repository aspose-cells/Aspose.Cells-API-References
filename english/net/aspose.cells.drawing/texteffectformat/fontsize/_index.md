---
title: TextEffectFormat.FontSize
second_title: Aspose.Cells for .NET API Reference
description: TextEffectFormat property. The size in points of the font used in the WordArt
type: docs
url: /net/aspose.cells.drawing/texteffectformat/fontsize/
---
## TextEffectFormat.FontSize property

The size (in points) of the font used in the WordArt.

```csharp
public int FontSize { get; set; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(effFormatSrc.FontSize, effFormatDest.FontSize, info + ".FontSize");
public static void Property_FontSize(TextEffectFormat effFormatSrc, TextEffectFormat effFormatDest, string info)
        {
            AssertHelper.AreEqual(effFormatSrc.Text, effFormatDest.Text, info + ".Text");
            AssertHelper.AreEqual(effFormatSrc.FontName, effFormatDest.FontName, info + ".FontName");
            AssertHelper.AreEqual(effFormatSrc.FontBold, effFormatDest.FontBold, info + ".FontBold");
            AssertHelper.AreEqual(effFormatSrc.FontItalic, effFormatDest.FontItalic, info + ".FontItalic");
            AssertHelper.AreEqual(effFormatSrc.FontSize, effFormatDest.FontSize, info + ".FontSize");
            AssertHelper.AreEqual(effFormatSrc.RotatedChars, effFormatDest.RotatedChars, info + ".RotatedChars");
            AssertHelper.AreEqual(effFormatSrc.PresetShape, effFormatDest.PresetShape, info + ".PresetShape");
        }
```

### See Also

* class [TextEffectFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


