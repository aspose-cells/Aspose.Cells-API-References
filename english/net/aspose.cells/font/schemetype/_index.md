---
title: Font.SchemeType
second_title: Aspose.Cells for .NET API Reference
description: Font property. Gets and sets the scheme type of the font
type: docs
url: /net/aspose.cells/font/schemetype/
---
## Font.SchemeType property

Gets and sets the scheme type of the font.

```csharp
public FontSchemeType SchemeType { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(source.SchemeType, dest.SchemeType);
public static void Property_SchemeType(Font source, Font dest)
        {
            bool isSourceNull = (source == null);
            bool isDestNull = (dest == null);
            Assert.AreEqual(isSourceNull, isDestNull);

            if (isSourceNull)
            {
                return;
            }
            Assert.AreEqual(source.Name, dest.Name);
            Assert.AreEqual(source.Size, dest.Size);
            Assert.AreEqual(source.SchemeType, dest.SchemeType);
            Assert.AreEqual(source.IsNormalizeHeights, dest.IsNormalizeHeights);
            Assert.AreEqual(source.IsItalic, dest.IsItalic);
            Assert.AreEqual(source.Charset, dest.Charset);
            Assert.AreEqual(source.Color, dest.Color);
            //Assert.AreEqual(source.IsBold, dest.IsBold);
            Assert.AreEqual(source.IsStrikeout, dest.IsStrikeout);
            Assert.AreEqual(source.IsSubscript, dest.IsSubscript);
            Assert.AreEqual(source.IsSuperscript, dest.IsSuperscript);
            Assert.AreEqual(source.ScriptOffset, dest.ScriptOffset);
            Assert.AreEqual(source.StrikeType, dest.StrikeType);
            //Assert.AreEqual(source.ThemeColor, dest.ThemeColor);
            Assert.AreEqual(source.Underline, dest.Underline);
        }
```

### See Also

* enum [FontSchemeType](../../fontschemetype/)
* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


