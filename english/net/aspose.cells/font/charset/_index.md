---
title: Font.Charset
second_title: Aspose.Cells for .NET API Reference
description: Font property. Represent the character set
type: docs
url: /net/aspose.cells/font/charset/
---
## Font.Charset property

Represent the character set.

```csharp
public int Charset { get; set; }
```

### Examples

```csharp
// Called: int c = style.Font.Charset;//CELLSNET-43128
[Test]
        public void Property_Charset()
        {
            caseName = &quot;testFont_001&quot;;
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            Style style = cells[0, 0].GetStyle();
            style.Font.Color = Color.Red;
            style.Font.Size = 12;
            style.Font.Name = &quot;Arial&quot;;
            style.Font.IsBold = true;
            style.Font.Underline = FontUnderlineType.Double;
            int c = style.Font.Charset;//CELLSNET-43128
            cells[0, 0].SetStyle(style);

            workbook.Save(Constants.destPath + &quot;testFont.xls&quot;);
            workbook = new Workbook(Constants.destPath + &quot;testFont.xls&quot;);
            checkFont_001(workbook);
            workbook.Save(Constants.destPath + &quot;testFont.xlsx&quot;);
            workbook = new Workbook(Constants.destPath + &quot;testFont.xlsx&quot;);
            checkFont_001(workbook);
            workbook.Save(Constants.destPath + &quot;testFont.xml&quot;, SaveFormat.SpreadsheetML);
            workbook = new Workbook(Constants.destPath + &quot;testFont.xml&quot;);
            checkFont_001(workbook);
            workbook.Save(Constants.destPath + &quot;testFont.xls&quot;);
        }
```

### See Also

* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


