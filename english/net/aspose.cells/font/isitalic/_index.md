---
title: Font.IsItalic
second_title: Aspose.Cells for .NET API Reference
description: Font property. Gets or sets a value indicating whether the font is italic
type: docs
url: /net/aspose.cells/font/isitalic/
---
## Font.IsItalic property

Gets or sets a value indicating whether the font is italic.

```csharp
public bool IsItalic { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(true, defaultstyle.Font.IsItalic);
public void Font_Property_IsItalic()
{
    SetDefaultStyle();
    Workbook workbook = new Workbook(Constants.destPath + "defaultstyle.xls");
    Style defaultstyle = workbook.DefaultStyle;
    //Number
    Assert.AreEqual("#,##0", defaultstyle.Custom);
    //Alignment
   Assert.AreEqual(TextAlignmentType.Left, defaultstyle.HorizontalAlignment);
    //Assert.AreEqual(TextAlignmentType.Left, defaultstyle.VerticalAlignment);
    Assert.AreEqual(5, defaultstyle.IndentLevel);
    Assert.AreEqual(TextDirectionType.LeftToRight, defaultstyle.TextDirection);
    Assert.AreEqual(true, defaultstyle.IsTextWrapped);
    Assert.AreEqual(true, defaultstyle.ShrinkToFit);
    Assert.AreEqual(30, defaultstyle.RotationAngle);
    //Font
    Assert.AreEqual("Tahoma", defaultstyle.Font.Name);
    Assert.AreEqual(16, defaultstyle.Font.Size);
    Assert.AreEqual(FontUnderlineType.Double, defaultstyle.Font.Underline);
    AssertHelper.equals(Color.Red, defaultstyle.Font.Color,"Font color");
    Assert.AreEqual(true, defaultstyle.Font.IsBold);
    Assert.AreEqual(true, defaultstyle.Font.IsItalic);
    Assert.AreEqual(true, defaultstyle.Font.IsSubscript);
    //Border
    AssertHelper.equals(Color.Blue, defaultstyle.Borders[BorderType.BottomBorder].Color,"border color");
    Assert.AreEqual(CellBorderType.Dashed, defaultstyle.Borders[BorderType.BottomBorder].LineStyle);
    Assert.AreEqual(false, defaultstyle.IsLocked);  
}
```

### See Also

* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


