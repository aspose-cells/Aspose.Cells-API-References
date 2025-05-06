---
title: Font.StrikeType
second_title: Aspose.Cells for .NET API Reference
description: Font property. Gets the strike type of the text
type: docs
url: /net/aspose.cells/font/striketype/
---
## Font.StrikeType property

Gets the strike type of the text.

```csharp
public TextStrikeType StrikeType { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(source.StrikeType, dest.StrikeType);
public static void Property_StrikeType(Font source, Font dest)
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

* enum [TextStrikeType](../../textstriketype/)
* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


