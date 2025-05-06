---
title: HtmlLoadOptions.AutoFitColsAndRows
second_title: Aspose.Cells for .NET API Reference
description: HtmlLoadOptions property. Indicates whether autofit columns and rows. The default value is false
type: docs
url: /net/aspose.cells/htmlloadoptions/autofitcolsandrows/
---
## HtmlLoadOptions.AutoFitColsAndRows property

Indicates whether auto-fit columns and rows. The default value is false.

```csharp
public bool AutoFitColsAndRows { get; set; }
```

### Examples

```csharp
// Called: options.AutoFitColsAndRows = true;
[Test]
        public void Property_AutoFitColsAndRows()
        {
            string filePath = Constants.JohnTest_PATH_SOURCE + @&quot;JAVA42256And42259/&quot;;
            HtmlLoadOptions options = new HtmlLoadOptions();
            options.AutoFitColsAndRows = true;
            Workbook workbook = null;
            Cells cells = null;
            workbook = new Workbook(filePath + &quot;new11.html&quot;, options);
            cells = workbook.Worksheets[0].Cells;

            Assert.AreEqual(cells[&quot;A1&quot;].StringValue, &quot;This is a false alarm for below reasons:&quot;);
            Assert.AreEqual(cells[&quot;A3&quot;].StringValue, &quot;1. Reason 1&quot;);
            Assert.AreEqual(cells[&quot;A6&quot;].StringValue, &quot;Attention: My Project Team, &quot;);
            Assert.AreEqual(cells[&quot;A12&quot;].StringValue, &quot;1. Customer count in the  File = 74&quot;);
            Cell a13 = cells[&quot;A13&quot;];
            Assert.AreEqual(a13.IsRichText(), true);
            Assert.AreEqual(a13.GetCharacters()[1].Font.StrikeType, TextStrikeType.Single);

            Cell a14 = cells[&quot;A14&quot;];
            Assert.AreEqual(a14.IsRichText(), true);
            Assert.AreEqual(a14.GetCharacters()[1].Font.Color, Color.FromArgb(255, 255, 240, 0));
            workbook.Save(CreateFolder(filePath) + &quot;java42256.xlsx&quot;);

            workbook = new Workbook(filePath + &quot;Single_Tab.html&quot;, options);
            cells = workbook.Worksheets[0].Cells;
            //If the H/P/OL/UL/LI tag is the first column, it is counted as a whole row. 
            //If it is in other columns, the H/P/OL/UL/LI tag text are arranged in the current cell
            Assert.AreEqual(cells[&quot;A1&quot;].StringValue, &quot;Customer Id&quot;);
            Assert.AreEqual(cells[&quot;B2&quot;].StringValue, &quot;One Sample Name&quot;);
            Assert.AreEqual(cells[&quot;A4&quot;].StringValue, &quot;ABCDTiger&quot;);
            Cell c4 = cells[&quot;C4&quot;];
            Assert.AreEqual(c4.IsRichText(), true);
            FontSetting[] characters = c4.GetCharacters();
            int charactersLen = characters.Length;
            Assert.AreEqual(characters[0].Font.Color, Color.FromArgb(255, 204, 0, 0));

            Assert.AreEqual(characters[charactersLen - 1].Font.Color, Color.FromArgb(255, 0, 128, 0));
            Assert.AreEqual(characters[charactersLen - 1].Font.Underline, FontUnderlineType.Single);

            //Assert.AreEqual(cells[&quot;A1&quot;].StringValue, &quot;Customer Id&quot;);
            //Assert.AreEqual(cells[&quot;B2&quot;].StringValue, &quot;One Sample Name&quot;);
            //Assert.AreEqual(cells[&quot;A4&quot;].StringValue, &quot;ABCDTiger&quot;);
            //Assert.AreEqual(cells[&quot;C12&quot;].StringValue, &quot;3. List3&quot;);
            //Cell c4 = cells[&quot;C4&quot;];
            //Assert.AreEqual(c4.GetStyle().Font.Color, Color.FromArgb(255, 204, 0, 0));
            //Cell c13 = cells[&quot;C13&quot;];
            //Assert.AreEqual(c13.GetStyle().Font.IsBold, true);

            //Cell c14 = cells[&quot;C14&quot;];
            //Assert.AreEqual(c14.GetStyle().Font.Color, Color.FromArgb(255, 255, 0, 0));
            //Assert.AreEqual(c14.GetStyle().Font.StrikeType, TextStrikeType.Single);
            //Cell c15 = cells[&quot;C15&quot;];
            //Assert.AreEqual(c15.GetStyle().Font.Color, Color.FromArgb(255, 0, 128, 0));
            //Assert.AreEqual(c15.GetStyle().Font.Underline, FontUnderlineType.Single);
            workbook.Save(CreateFolder(filePath) + &quot;java42259.xlsx&quot;);
        }
```

### See Also

* class [HtmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


