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
// Called: AssertHelper.AreEqual(effFormatSrc.FontBold, effFormatDest.FontBold, info + ".FontBold");
public static void Property_FontBold(TextEffectFormat effFormatSrc, TextEffectFormat effFormatDest, string info)
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


