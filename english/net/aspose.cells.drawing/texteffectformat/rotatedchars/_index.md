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
// Called: AssertHelper.AreEqual(effFormatSrc.RotatedChars, effFormatDest.RotatedChars, info + &amp;quot;.RotatedChars&amp;quot;);
public static void Property_RotatedChars(TextEffectFormat effFormatSrc, TextEffectFormat effFormatDest, string info)
        {
            AssertHelper.AreEqual(effFormatSrc.Text, effFormatDest.Text, info + &quot;.Text&quot;);
            AssertHelper.AreEqual(effFormatSrc.FontName, effFormatDest.FontName, info + &quot;.FontName&quot;);
            AssertHelper.AreEqual(effFormatSrc.FontBold, effFormatDest.FontBold, info + &quot;.FontBold&quot;);
            AssertHelper.AreEqual(effFormatSrc.FontItalic, effFormatDest.FontItalic, info + &quot;.FontItalic&quot;);
            AssertHelper.AreEqual(effFormatSrc.FontSize, effFormatDest.FontSize, info + &quot;.FontSize&quot;);
            AssertHelper.AreEqual(effFormatSrc.RotatedChars, effFormatDest.RotatedChars, info + &quot;.RotatedChars&quot;);
            AssertHelper.AreEqual(effFormatSrc.PresetShape, effFormatDest.PresetShape, info + &quot;.PresetShape&quot;);
        }
```

### See Also

* class [TextEffectFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


