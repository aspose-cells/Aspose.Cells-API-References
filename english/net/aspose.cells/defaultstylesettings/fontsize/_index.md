---
title: DefaultStyleSettings.FontSize
second_title: Aspose.Cells for .NET API Reference
description: DefaultStyleSettings property. Gets/Sets the default standard font size for the workbook
type: docs
url: /net/aspose.cells/defaultstylesettings/fontsize/
---
## DefaultStyleSettings.FontSize property

Gets/Sets the default standard font size for the workbook.

```csharp
public double FontSize { get; set; }
```

### Examples

```csharp
// Called: htmlLoadOptions.DefaultStyleSettings.FontSize = 11.0;
public void DefaultStyleSettings_Property_FontSize()
{
    HtmlLoadOptions htmlLoadOptions = new HtmlLoadOptions();

    htmlLoadOptions.DefaultStyleSettings.FontName = "Calibri";
    htmlLoadOptions.DefaultStyleSettings.FontSize = 11.0;

    Workbook workbook = new Workbook(Constants.HtmlPath + "example.html", htmlLoadOptions);

    Assert.AreEqual(FontSchemeType.None, workbook.Worksheets[0].Cells["B3"].GetStyle().Font.SchemeType);
}
```

### See Also

* class [DefaultStyleSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


