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
public void ReplaceOptions_Property_StyleFlags()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
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
           
    workbook.Save(Constants.destPath + "example.xlsx");
}
```

### See Also

* class [StyleFlag](../../styleflag/)
* class [ReplaceOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


