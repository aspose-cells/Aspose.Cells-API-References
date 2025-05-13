---
title: FontSetting.Font
second_title: Aspose.Cells for .NET API Reference
description: FontSetting property. Returns the font of this object
type: docs
url: /net/aspose.cells/fontsetting/font/
---
## FontSetting.Font property

Returns the font of this object.

```csharp
public Font Font { get; }
```

### Examples

```csharp
// Called: cell.Characters(46, 30).Font.IsItalic = true;
public void FontSetting_Property_Font()
{
    Workbook workbook = new Workbook();
    Cell cell = workbook.Worksheets[0].Cells["A1"];
    cell.PutValue("Hello. I have Bold texts in blue without any italicized textthat isn't bold last stuff unformatted");
    cell.Characters(15, 4).Font.IsBold = true;
    cell.Characters(29, 4).Font.Color = ColorTranslator.FromHtml("blue");
    cell.Characters(33, 16).Font.Color = ColorTranslator.FromHtml("green");
    cell.Characters(38, 3).Font.IsStrikeout = true;
    cell.Characters(46, 15).Font.IsBold = true;
    cell.Characters(46, 30).Font.IsItalic = true;
    workbook.Save(Constants.destPath + "example.xls");
    workbook = new Workbook(Constants.destPath + "example.xls");
    cell = workbook.Worksheets[0].Cells["A1"];
    FontSetting[] chs = cell.GetCharacters();
    for (int i = 0; i < chs.Length; i++)
    {
        FontSetting chars = (FontSetting)chs[i];
        if (chars.StartIndex == 46)
        {
           Assert.AreEqual(chars.Length,3);
           Assert.AreEqual(chars.Font.IsBold,true);
           Assert.AreEqual(chars.Font.IsItalic,true);
        }

    }
}
```

### See Also

* class [Font](../../font/)
* class [FontSetting](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


