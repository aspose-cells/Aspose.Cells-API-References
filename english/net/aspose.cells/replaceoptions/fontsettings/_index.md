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
// Called: options.FontSettings = settingsList.ToArray();
[Test]
        public void Property_FontSettings()
        {
            bool caseSensitive = false;
            bool matchEntireCellContents = false;
            string searchText = &quot;Dickens&quot;;
            string regText = &quot;^[pbtd][^aeiou]&quot;;
            string replacementText = &quot;Hulahoop&quot;;
            bool useRegex = false;
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;Replace001.xlsx&quot;);
            ReplaceOptions options = new ReplaceOptions();

            // Set case sensitivity and text matching options
            options.CaseSensitive = caseSensitive;
            options.MatchEntireCellContents = matchEntireCellContents;

            List&lt;Aspose.Cells.FontSetting&gt; settingsList = new List&lt;Aspose.Cells.FontSetting&gt;(); // replace.FontSettings.ToList();
            Aspose.Cells.FontSetting setting = new Aspose.Cells.FontSetting(0, replacementText.Length, workbook.Worksheets);

            //setting.Font.IsBold = true; // ExcelFont.IsBold;
            setting.Font.Color = System.Drawing.Color.Red; //ExcelFont.Color
                                                           //setting.Font.Size = 22;
                                                           //setting.Font.Name = &quot;ALGERIAN&quot;;


            setting.Font.Underline = Aspose.Cells.FontUnderlineType.Single;

            setting.Font.IsStrikeout = true;
            setting.Font.StrikeType = Aspose.Cells.TextStrikeType.Double;

            settingsList.Add(setting);
            options.FontSettings = settingsList.ToArray();

            if (!useRegex)
            {
                // Replace text
                workbook.Replace(searchText, replacementText, options);
            }
            else
            {
                options.RegexKey = true;
                workbook.Replace(regText, replacementText, options);
            }

            FontSetting fs = workbook.Worksheets[0].Cells[&quot;B1&quot;].Characters(&quot;wo shi &quot;.Length, replacementText.Length);
            Assert.IsTrue(fs.Font.IsStrikeout);
        }
```

### See Also

* class [FontSetting](../../fontsetting/)
* class [ReplaceOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


