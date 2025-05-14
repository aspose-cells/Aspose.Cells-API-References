---
title: Font.Color
second_title: Aspose.Cells for .NET API Reference
description: Font property. Gets or sets the Color of the font
type: docs
url: /net/aspose.cells/font/color/
---
## Font.Color property

Gets or sets the Color of the font.

```csharp
public Color Color { get; set; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(richText[1].Font.Color, Color.FromArgb(0xb71c1c));
public void Font_Property_Color()
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

    workbook.Save(Constants.destPath + "example.xlsx");
}
```

### See Also

* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


