---
title: LoadOptions.DefaultStyleSettings
second_title: Aspose.Cells for .NET API Reference
description: LoadOptions property. Gets the default style settings for initializing styles of the workbook
type: docs
url: /net/aspose.cells/loadoptions/defaultstylesettings/
---
## LoadOptions.DefaultStyleSettings property

Gets the default style settings for initializing styles of the workbook

```csharp
public DefaultStyleSettings DefaultStyleSettings { get; }
```

### Examples

```csharp
// Called: loadOptions.DefaultStyleSettings.FontName = &amp;quot;SimSun&amp;quot;;
[Test]
        public void Property_DefaultStyleSettings()
        {
            LoadOptions loadOptions = new LoadOptions();
            loadOptions.DefaultStyleSettings.FontName = &quot;SimSun&quot;;
            loadOptions.Region = CountryCode.USA;
            loadOptions.MemorySetting = MemorySetting.MemoryPreference;
            Workbook excel = new Workbook(Constants.HtmlPath + &quot;CELLSJAVA-43812.xlsx&quot;, loadOptions);
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
                Assert.IsTrue(reLoadWb.Worksheets[0].Shapes[0].UpperLeftColumn &gt;= 15);
            }
        }
```

### See Also

* class [DefaultStyleSettings](../../defaultstylesettings/)
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


