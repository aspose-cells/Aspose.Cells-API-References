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
// Called: options.FontSettings = new FontSetting[] { setting1 };
public void ReplaceOptions_Property_FontSettings()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");

    string text = "asdf";
    string replacementText = "text";

    ReplaceOptions options = new ReplaceOptions();
    options.MatchEntireCellContents = false;
    FontSetting setting1 = new FontSetting(0, replacementText.Length, workbook.Worksheets);
    setting1.Font.IsBold = true;
    setting1.Font.Color = System.Drawing.Color.Blue;
    options.FontSettings = new FontSetting[] { setting1 };

    workbook.Replace(text, replacementText, options);


    FontSetting fs = workbook.Worksheets[0].Cells["B1"].Characters(3, 4);
   Assert.IsTrue(Util.CompareColor(Color.Blue, fs.Font.Color));
    Assert.IsTrue(fs.Font.IsBold);

    workbook.Save(Constants.destPath + "example.xlsx");
}
```

### See Also

* class [FontSetting](../../fontsetting/)
* class [ReplaceOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


