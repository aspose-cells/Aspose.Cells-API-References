---
title: TextEffectFormat.RotatedChars
second_title: Aspose.Cells for .NET API Reference
description: TextEffectFormat property. If truecharacters in the specified WordArt are rotated 90 degrees relative to the WordArts bounding shape
type: docs
url: /net/aspose.cells.drawing/texteffectformat/rotatedchars/
---
## TextEffectFormat.RotatedChars property

If true,characters in the specified WordArt are rotated 90 degrees relative to the WordArt's bounding shape.

```csharp
public bool RotatedChars { get; set; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(effFormatSrc.RotatedChars, effFormatDest.RotatedChars, info + ".RotatedChars");
public static void Property_RotatedChars(TextEffectFormat effFormatSrc, TextEffectFormat effFormatDest, string info)
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


