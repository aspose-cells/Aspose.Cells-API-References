---
title: TextEffectFormat.FontBold
second_title: Aspose.Cells for .NET API Reference
description: TextEffectFormat property. Indicates whether font is bold
type: docs
url: /net/aspose.cells.drawing/texteffectformat/fontbold/
---
## TextEffectFormat.FontBold property

Indicates whether font is bold.

```csharp
public bool FontBold { get; set; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(effFormatSrc.FontBold, effFormatDest.FontBold, info + &amp;quot;.FontBold&amp;quot;);
public static void Property_FontBold(TextEffectFormat effFormatSrc, TextEffectFormat effFormatDest, string info)
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


