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
            Cell cell = wb.Worksheets[0].Cells["A1"];
            cell.Value = "rich text with color";
            FontSetting fontSetting = new FontSetting(1, 7, wb.Worksheets);
            fontSetting.Font.Color = Color.Red;
            cell.SetCharacters(new FontSetting[] { fontSetting });

            cell = wb.Worksheets[0].Cells["A2"];
            cell.Value = "different font";
            Style style = cell.GetStyle();
            style.Font.Name = "Times New Roman";
            style.Font.Size = 24;
            cell.SetStyle(style);

            HtmlSaveOptions htmlSaveOptions = new HtmlSaveOptions();
            htmlSaveOptions.ExcludeUnusedStyles = true;

            string savePath = _destFilesPath + "CELLSNET-50531.html";
            wb.Save(savePath, htmlSaveOptions);

            string content = File.ReadAllText(savePath);
            Assert.IsTrue(content.IndexOf(".font0") > -1);
            Assert.IsTrue(content.IndexOf(".font2") > -1);
            Assert.IsTrue(content.IndexOf(".font1") == -1);

        }
```

### See Also

* class [WorksheetCollection](../../worksheetcollection/)
* class [FontSetting](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


