---
title: Font.IsStrikeout
second_title: Aspose.Cells for .NET API Reference
description: Font property. Gets or sets a value indicating whether the font is single strikeout
type: docs
url: /net/aspose.cells/font/isstrikeout/
---
## Font.IsStrikeout property

Gets or sets a value indicating whether the font is single strikeout.

```csharp
public bool IsStrikeout { get; set; }
```

### Examples

```csharp
// Called: Assert.IsTrue(richText[1].Font.IsStrikeout);
[Test]
        public void Property_IsStrikeout()
        {
            Workbook workbook = new Workbook();

            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Code");


            Cell cell = worksheet.Cells["A2"];
            cell.HtmlString = "<pre><font color='Green'>/*---------------------------------------------------------------------------------------<br />" +
                             "<font style='color: #b71c1c;text-decoration: line-through;'>Auther :</font>" +
                             "<font color='Green'>Author :</font>---------------------------------------------------------------------------------------*/<br /> <br /></font>";
           // cell.HtmlString = "<s><span style=\"color:#ff00ff;\">S2</span></s>";
            // cell.SetStyle(style);
            // Saving the Excel file
            FontSetting[] richText = cell.GetCharacters();
           AssertHelper.AreEqual(richText[1].Font.Color, Color.FromArgb(0xb71c1c));
            Assert.IsTrue(richText[1].Font.IsStrikeout);

           AssertHelper.AreEqual(richText[3].Font.Color, Color.Green);
            Assert.IsFalse(richText[3].Font.IsStrikeout);

            workbook.Save(Constants.destPath + "CELLSNET45326.xlsx");
        }
```

### See Also

* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


