---
title: FontSetting.FontSetting
second_title: Aspose.Cells for .NET API Reference
description: FontSetting constructor. 
type: docs
url: /net/aspose.cells/fontsetting/fontsetting/
---
## FontSetting constructor

```csharp
public FontSetting(int startIndex, int length, WorksheetCollection sheets)
```

| Parameter | Type | Description |
| --- | --- | --- |
| startIndex | Int32 |  |
| length | Int32 |  |
| sheets | WorksheetCollection |  |

### Examples

```csharp
// Called: FontSetting fontSetting = new FontSetting(1, 7, wb.Worksheets);
[Test]
        public void FontSetting_Constructor()
        {
            Workbook wb = new Workbook();
            Cell cell = wb.Worksheets[0].Cells[&quot;A1&quot;];
            cell.Value = &quot;rich text with color&quot;;
            FontSetting fontSetting = new FontSetting(1, 7, wb.Worksheets);
            fontSetting.Font.Color = Color.Red;
            cell.SetCharacters(new FontSetting[] { fontSetting });

            cell = wb.Worksheets[0].Cells[&quot;A2&quot;];
            cell.Value = &quot;different font&quot;;
            Style style = cell.GetStyle();
            style.Font.Name = &quot;Times New Roman&quot;;
            style.Font.Size = 24;
            cell.SetStyle(style);

            HtmlSaveOptions htmlSaveOptions = new HtmlSaveOptions();
            htmlSaveOptions.ExcludeUnusedStyles = true;

            string savePath = _destFilesPath + &quot;CELLSNET-50531.html&quot;;
            wb.Save(savePath, htmlSaveOptions);

            string content = File.ReadAllText(savePath);
            Assert.IsTrue(content.IndexOf(&quot;.font0&quot;) &gt; -1);
            Assert.IsTrue(content.IndexOf(&quot;.font2&quot;) &gt; -1);
            Assert.IsTrue(content.IndexOf(&quot;.font1&quot;) == -1);

        }
```

### See Also

* class [WorksheetCollection](../../worksheetcollection/)
* class [FontSetting](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


