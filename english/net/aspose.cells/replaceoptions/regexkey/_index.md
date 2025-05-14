---
title: ReplaceOptions.RegexKey
second_title: Aspose.Cells for .NET API Reference
description: ReplaceOptions property. Indicates whether the searched key is regex. If true then the searched key will be taken as regex
type: docs
url: /net/aspose.cells/replaceoptions/regexkey/
---
## ReplaceOptions.RegexKey property

Indicates whether the searched key is regex. If true then the searched key will be taken as regex.

```csharp
public bool RegexKey { get; set; }
```

### Examples

```csharp
// Called: options.RegexKey = true;
public void ReplaceOptions_Property_RegexKey()
{
    bool caseSensitive = false;
    bool matchEntireCellContents = false;
    string searchText = "Dickens";
    string regText = "^[pbtd][^aeiou]";
    string replacementText = "Hulahoop";
    bool useRegex = false;
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    ReplaceOptions options = new ReplaceOptions();

    // Set case sensitivity and text matching options
    options.CaseSensitive = caseSensitive;
    options.MatchEntireCellContents = matchEntireCellContents;

    List<Aspose.Cells.FontSetting> settingsList = new List<Aspose.Cells.FontSetting>(); // replace.FontSettings.ToList();
    Aspose.Cells.FontSetting setting = new Aspose.Cells.FontSetting(0, replacementText.Length, workbook.Worksheets);

    //setting.Font.IsBold = true; // ExcelFont.IsBold;
    setting.Font.Color = System.Drawing.Color.Red; //ExcelFont.Color
                                                   //setting.Font.Size = 22;
                                                   //setting.Font.Name = "ALGERIAN";


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

    FontSetting fs = workbook.Worksheets[0].Cells["B1"].Characters("wo shi ".Length, replacementText.Length);
    Assert.IsTrue(fs.Font.IsStrikeout);
}
```

### See Also

* class [ReplaceOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


