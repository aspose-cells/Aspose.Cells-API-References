---
title: Font.Charset
second_title: Aspose.Cells for .NET API Reference
description: Font property. Represent the character set
type: docs
url: /net/aspose.cells/font/charset/
---
## Font.Charset property

Represent the character set.

```csharp
public int Charset { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(source.Charset, dest.Charset);
public static void Font_Property_Charset(Font source, Font dest)
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

* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


