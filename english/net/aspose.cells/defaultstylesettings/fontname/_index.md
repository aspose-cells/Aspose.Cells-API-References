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
// Called: loadOptions.DefaultStyleSettings.FontName = "SimSun";
public void DefaultStyleSettings_Property_FontName()
{
    LoadOptions loadOptions = new LoadOptions();
    loadOptions.DefaultStyleSettings.FontName = "SimSun";
    loadOptions.Region = CountryCode.USA;
    loadOptions.MemorySetting = MemorySetting.MemoryPreference;
    Workbook excel = new Workbook(Constants.HtmlPath + "example.xlsx", loadOptions);
    excel.AcceptAllRevisions();
    HtmlSaveOptions saveOptions = new HtmlSaveOptions();
    saveOptions.ExportActiveWorksheetOnly = true;
    saveOptions.ExportHiddenWorksheet = false;
    saveOptions.ExportImagesAsBase64 = true;
    saveOptions.HiddenColDisplayType = HtmlHiddenColDisplayType.Hidden;
    saveOptions.HiddenRowDisplayType = HtmlHiddenRowDisplayType.Hidden;
    saveOptions.LinkTargetType = HtmlLinkTargetType.Blank;

    saveOptions.ExcludeUnusedStyles = true;


    using (MemoryStream ms = new MemoryStream())
    {
        excel.Save(ms, saveOptions);
        ms.Position = 0;

        Workbook reLoadWb = new Workbook(ms);
        Assert.IsTrue(reLoadWb.Worksheets[0].Shapes[0].UpperLeftColumn >= 15);
    }
}
```

### See Also

* class [DefaultStyleSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


