---
title: Font.StrikeType
second_title: Aspose.Cells for .NET API Reference
description: Font property. Gets the strike type of the text
type: docs
url: /net/aspose.cells/font/striketype/
---
## Font.StrikeType property

Gets the strike type of the text.

```csharp
public TextStrikeType StrikeType { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(a13.GetCharacters()[1].Font.StrikeType, TextStrikeType.Single);
public void Font_Property_StrikeType()
{
    string filePath = Constants.JohnTest_PATH_SOURCE + @"JAVA42256And42259/";
    HtmlLoadOptions options = new HtmlLoadOptions();
    options.AutoFitColsAndRows = true;
    Workbook workbook = null;
    Cells cells = null;
    workbook = new Workbook(filePath + "example.html", options);
    cells = workbook.Worksheets[0].Cells;

    Assert.AreEqual(cells["A1"].StringValue, "This is a false alarm for below reasons:");
    Assert.AreEqual(cells["A3"].StringValue, "1. Reason 1");
    Assert.AreEqual(cells["A6"].StringValue, "Attention: My Project Team, ");
    Assert.AreEqual(cells["A12"].StringValue, "1. Customer count in the  File = 74");
    Cell a13 = cells["A13"];
    Assert.AreEqual(a13.IsRichText(), true);
    Assert.AreEqual(a13.GetCharacters()[1].Font.StrikeType, TextStrikeType.Single);

    Cell a14 = cells["A14"];
    Assert.AreEqual(a14.IsRichText(), true);
    Assert.AreEqual(a14.GetCharacters()[1].Font.Color, Color.FromArgb(255, 255, 240, 0));
    workbook.Save(CreateFolder(filePath) + "example.xlsx");

    workbook = new Workbook(filePath + "Single_Tab.html", options);
    cells = workbook.Worksheets[0].Cells;
    //If the H/P/OL/UL/LI tag is the first column, it is counted as a whole row. 
    //If it is in other columns, the H/P/OL/UL/LI tag text are arranged in the current cell
    Assert.AreEqual(cells["A1"].StringValue, "Customer Id");
    Assert.AreEqual(cells["B2"].StringValue, "One Sample Name");
    Assert.AreEqual(cells["A4"].StringValue, "ABCDTiger");
    Cell c4 = cells["C4"];
    Assert.AreEqual(c4.IsRichText(), true);
    FontSetting[] characters = c4.GetCharacters();
    int charactersLen = characters.Length;
    Assert.AreEqual(characters[0].Font.Color, Color.FromArgb(255, 204, 0, 0));

    Assert.AreEqual(characters[charactersLen - 1].Font.Color, Color.FromArgb(255, 0, 128, 0));
    Assert.AreEqual(characters[charactersLen - 1].Font.Underline, FontUnderlineType.Single);

    //Assert.AreEqual(cells["A1"].StringValue, "Customer Id");
    //Assert.AreEqual(cells["B2"].StringValue, "One Sample Name");
    //Assert.AreEqual(cells["A4"].StringValue, "ABCDTiger");
    //Assert.AreEqual(cells["C12"].StringValue, "3. List3");
    //Cell c4 = cells["C4"];
    //Assert.AreEqual(c4.GetStyle().Font.Color, Color.FromArgb(255, 204, 0, 0));
    //Cell c13 = cells["C13"];
    //Assert.AreEqual(c13.GetStyle().Font.IsBold, true);

    //Cell c14 = cells["C14"];
    //Assert.AreEqual(c14.GetStyle().Font.Color, Color.FromArgb(255, 255, 0, 0));
    //Assert.AreEqual(c14.GetStyle().Font.StrikeType, TextStrikeType.Single);
    //Cell c15 = cells["C15"];
    //Assert.AreEqual(c15.GetStyle().Font.Color, Color.FromArgb(255, 0, 128, 0));
    //Assert.AreEqual(c15.GetStyle().Font.Underline, FontUnderlineType.Single);
    workbook.Save(CreateFolder(filePath) + "example.xlsx");
}
```

### See Also

* enum [TextStrikeType](../../textstriketype/)
* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


