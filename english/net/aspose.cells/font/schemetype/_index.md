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
// Called: Assert.AreEqual(FontSchemeType.None, workbook.Worksheets[0].Cells[&amp;quot;B3&amp;quot;].GetStyle().Font.SchemeType);
[Test]
        public void Property_SchemeType()
        {
            HtmlLoadOptions htmlLoadOptions = new HtmlLoadOptions();

            htmlLoadOptions.DefaultStyleSettings.FontName = &quot;Calibri&quot;;
            htmlLoadOptions.DefaultStyleSettings.FontSize = 11.0;

            Workbook workbook = new Workbook(Constants.HtmlPath + &quot;CELLSJAVA-43792.html&quot;, htmlLoadOptions);

            Assert.AreEqual(FontSchemeType.None, workbook.Worksheets[0].Cells[&quot;B3&quot;].GetStyle().Font.SchemeType);
        }
```

### See Also

* enum [FontSchemeType](../../fontschemetype/)
* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


