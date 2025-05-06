---
title: ReplaceOptions.StyleFlags
second_title: Aspose.Cells for .NET API Reference
description: ReplaceOptions property. Gets and sets flags of applying font settings
type: docs
url: /net/aspose.cells/replaceoptions/styleflags/
---
## ReplaceOptions.StyleFlags property

Gets and sets flags of applying font settings.

```csharp
public StyleFlag[] StyleFlags { get; set; }
```

### Examples

```csharp
// Called: options.StyleFlags = new StyleFlag[] { styleFlag };
[Test]
        public void Property_StyleFlags()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CELLSNET57193.xlsx&quot;);
            string ReplacementText = &quot;wrongstyle&quot;;
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
            workbook.Replace(&quot;test&quot;, ReplacementText, options);
            Cell cell = workbook.Worksheets[0].Cells[&quot;C3&quot;];
            Assert.AreEqual(FontUnderlineType.Single, cell.Characters(0, &quot;wrongstyle&quot;.Length).Font.Underline);
           
            workbook.Save(Constants.destPath + &quot;CELLSNET57193.xlsx&quot;);
        }
```

### See Also

* class [StyleFlag](../../styleflag/)
* class [ReplaceOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


