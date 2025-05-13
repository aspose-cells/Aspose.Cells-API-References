---
title: Font.ThemeColor
second_title: Aspose.Cells for .NET API Reference
description: Font property. Gets and sets the theme color
type: docs
url: /net/aspose.cells/font/themecolor/
---
## Font.ThemeColor property

Gets and sets the theme color.

```csharp
public ThemeColor ThemeColor { get; set; }
```

### Remarks

If the font color is not a theme color, NULL will be returned.

### Examples

```csharp
// Called: ThemeColorTest.equals(fontSrc.ThemeColor, fontDest.ThemeColor, info + ".ThemeColor");
public static void Font_Property_ThemeColor(Font fontSrc, Font fontDest, string info)
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
            AssertHelper.Font_Property_ThemeColor(fontSrc.Color, fontDest.Color, info + ".Color");
            //===============properties are supported in excel 2007 format file=========//
            if(fontSrc.ThemeColor != null && fontDest.ThemeColor != null)
                ThemeColorTest.Font_Property_ThemeColor(fontSrc.ThemeColor, fontDest.ThemeColor, info + ".ThemeColor");
            
        }
```

### See Also

* class [ThemeColor](../../themecolor/)
* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


