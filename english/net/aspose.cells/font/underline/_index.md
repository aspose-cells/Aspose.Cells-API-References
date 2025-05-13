---
title: Font.Underline
second_title: Aspose.Cells for .NET API Reference
description: Font property. Gets or sets the font underline type
type: docs
url: /net/aspose.cells/font/underline/
---
## Font.Underline property

Gets or sets the font underline type.

```csharp
public FontUnderlineType Underline { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(sheet.Cells["B3"].GetStyle().Font.Underline, FontUnderlineType.None);
public void Font_Property_Underline()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "SpreadsheetWithHyperlinks.xlsm");
    Worksheet sheet = workbook.Worksheets[0];
    sheet.Hyperlinks.RemoveAt(0);
    Assert.AreEqual(sheet.Cells["B3"].GetStyle().Font.Underline, FontUnderlineType.None);
}
```

### See Also

* enum [FontUnderlineType](../../fontunderlinetype/)
* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


