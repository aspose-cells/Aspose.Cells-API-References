---
title: ReplaceOptions.FontSettings
second_title: Aspose.Cells for .NET API Reference
description: ReplaceOptions property. The rich formatted settings for the replaced text
type: docs
url: /net/aspose.cells/replaceoptions/fontsettings/
---
## ReplaceOptions.FontSettings property

The rich formatted settings for the replaced text.

```csharp
public FontSetting[] FontSettings { get; set; }
```

### Examples

```csharp
// Called: options.FontSettings = new FontSetting[] { setting };
[Test]
        public void Property_FontSettings()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CELLSNET57193.xlsx");
            string ReplacementText = "wrongstyle";
            FontSetting setting = new FontSetting(0, ReplacementText.Length, workbook.Worksheets);
            StyleFlag styleFlag = new StyleFlag();
            #region Set Up Options
            ReplaceOptions options = new ReplaceOptions();
            options.MatchEntireCellContents = false;
            options.CaseSensitive = false;


            setting.Font.Color = Color.Red;
            styleFlag.FontColor = true;
            options.FontSettings = new FontSetting[] { setting };
            options.StyleFlags = new StyleFlag[] { styleFlag };
            #endregion

            // Replace Text
            workbook.Replace("test", ReplacementText, options);
            Cell cell = workbook.Worksheets[0].Cells["C3"];
            Assert.AreEqual(FontUnderlineType.Single, cell.Characters(0, "wrongstyle".Length).Font.Underline);
           
            workbook.Save(Constants.destPath + "CELLSNET57193.xlsx");
        }
```

### See Also

* class [FontSetting](../../fontsetting/)
* class [ReplaceOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


