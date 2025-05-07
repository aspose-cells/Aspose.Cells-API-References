---
title: TextEffectFormat.PresetShape
second_title: Aspose.Cells for .NET API Reference
description: TextEffectFormat property. Gets and sets the preset shape type
type: docs
url: /net/aspose.cells.drawing/texteffectformat/presetshape/
---
## TextEffectFormat.PresetShape property

Gets and sets the preset shape type.

```csharp
public MsoPresetTextEffectShape PresetShape { get; set; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(effFormatSrc.PresetShape, effFormatDest.PresetShape, info + ".PresetShape");
public static void Property_PresetShape(TextEffectFormat effFormatSrc, TextEffectFormat effFormatDest, string info)
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

* enum [MsoPresetTextEffectShape](../../msopresettexteffectshape/)
* class [TextEffectFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


