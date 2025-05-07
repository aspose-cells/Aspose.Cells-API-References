---
title: DefaultStyleSettings.FontName
second_title: Aspose.Cells for .NET API Reference
description: DefaultStyleSettings property. Gets/Sets the default font name for the workbook
type: docs
url: /net/aspose.cells/defaultstylesettings/fontname/
---
## DefaultStyleSettings.FontName property

Gets/Sets the default font name for the workbook

```csharp
public string FontName { get; set; }
```

### Examples

```csharp
// Called: htmlLoadOptions.DefaultStyleSettings.FontName = "Calibri";
[Test]
        public void Property_FontName()
        {
            HtmlLoadOptions htmlLoadOptions = new HtmlLoadOptions();

            htmlLoadOptions.DefaultStyleSettings.FontName = "Calibri";
            htmlLoadOptions.DefaultStyleSettings.FontSize = 11.0;

            Workbook workbook = new Workbook(Constants.HtmlPath + "CELLSJAVA-43792.html", htmlLoadOptions);

            Assert.AreEqual(FontSchemeType.None, workbook.Worksheets[0].Cells["B3"].GetStyle().Font.SchemeType);
        }
```

### See Also

* class [DefaultStyleSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


