---
title: FontSetting.StartIndex
second_title: Aspose.Cells for .NET API Reference
description: FontSetting property. Gets the start index of the characters
type: docs
url: /net/aspose.cells/fontsetting/startindex/
---
## FontSetting.StartIndex property

Gets the start index of the characters.

```csharp
public int StartIndex { get; }
```

### Examples

```csharp
// Called: if (chars.StartIndex == 46)
[Test]
        public void Property_StartIndex()
        {
            Workbook workbook = new Workbook();
            Cell cell = workbook.Worksheets[0].Cells[&quot;A1&quot;];
            cell.PutValue(&quot;Hello. I have Bold texts in blue without any italicized textthat isn&apos;t bold last stuff unformatted&quot;);
            cell.Characters(15, 4).Font.IsBold = true;
            cell.Characters(29, 4).Font.Color = ColorTranslator.FromHtml(&quot;blue&quot;);
            cell.Characters(33, 16).Font.Color = ColorTranslator.FromHtml(&quot;green&quot;);
            cell.Characters(38, 3).Font.IsStrikeout = true;
            cell.Characters(46, 15).Font.IsBold = true;
            cell.Characters(46, 30).Font.IsItalic = true;
            workbook.Save(Constants.destPath + &quot;Test_160131.xls&quot;);
            workbook = new Workbook(Constants.destPath + &quot;Test_160131.xls&quot;);
            cell = workbook.Worksheets[0].Cells[&quot;A1&quot;];
            FontSetting[] chs = cell.GetCharacters();
            for (int i = 0; i &lt; chs.Length; i++)
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

* class [FontSetting](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


