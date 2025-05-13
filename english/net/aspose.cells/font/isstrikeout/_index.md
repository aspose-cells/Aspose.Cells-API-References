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
// Called: Assert.AreEqual(a1.GetStyle().Font.IsStrikeout, true);
public void Font_Property_IsStrikeout()
{
    Workbook workbook = new Workbook();


    Worksheet worksheet = workbook.Worksheets[0];


    Cell a1 = worksheet.Cells["A1"];


    //a1.setHtmlString("<span style=\"color:#ff00ff;\"><s>F1</s></span>");//it works 

    a1.HtmlString = ("<s><span style=\"color:#ff00ff;\">S2</span></s>");//it does not work 
    Assert.AreEqual(a1.GetStyle().Font.IsStrikeout, true);

}
```

### See Also

* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


