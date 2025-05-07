---
title: Font.IsSubscript
second_title: Aspose.Cells for .NET API Reference
description: Font property. Gets or sets a value indicating whether the font is subscript
type: docs
url: /net/aspose.cells/font/issubscript/
---
## Font.IsSubscript property

Gets or sets a value indicating whether the font is subscript.

```csharp
public bool IsSubscript { get; set; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(fontSrc.IsSubscript, fontDest.IsSubscript, info + ".IsSubscript");
public static void Property_IsSubscript(Font fontSrc, Font fontDest, string info)
        {
            if (AssertHelper.checkNull(fontSrc, fontDest, info))
            {
                return;
            }
            //===============properties are supported in excel 2003 format file========//
            AssertHelper.AreEqual(fontSrc.Name, fontDest.Name, info + ".Name");
            AssertHelper.AreEqual(fontSrc.Size, fontDest.Size, info + ".Size");
            AssertHelper.AreEqual(fontSrc.Underline, fontDest.Underline, info + ".Underline");
            AssertHelper.AreEqual(fontSrc.IsBold, fontDest.IsBold, info + ".IsBold");
            AssertHelper.AreEqual(fontSrc.IsItalic, fontDest.IsItalic, info + ".IsItalic");
            AssertHelper.AreEqual(fontSrc.IsStrikeout, fontDest.IsStrikeout, info + ".IsStrikeout");
            AssertHelper.AreEqual(fontSrc.IsSubscript, fontDest.IsSubscript, info + ".IsSubscript");
            AssertHelper.AreEqual(fontSrc.IsSuperscript, fontDest.IsSuperscript, info + ".IsSuperscript");
            AssertHelper.Property_IsSubscript(fontSrc.Color, fontDest.Color, info + ".Color");
            //===============properties are supported in excel 2007 format file=========//
            if(fontSrc.ThemeColor != null && fontDest.ThemeColor != null)
                ThemeColorTest.Property_IsSubscript(fontSrc.ThemeColor, fontDest.ThemeColor, info + ".ThemeColor");
            
        }
```

### See Also

* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


