---
title: Font.IsBold
second_title: Aspose.Cells for .NET API Reference
description: Font property. Gets or sets a value indicating whether the font is bold
type: docs
url: /net/aspose.cells/font/isbold/
---
## Font.IsBold property

Gets or sets a value indicating whether the font is bold.

```csharp
public bool IsBold { get; set; }
```

### Examples

```csharp
// Called: Assert.IsTrue(style.Font.IsBold);
public void Font_Property_IsBold()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.ods");
    workbook.Save(Constants.destPath + "example.xlsx");
    workbook= new Workbook(Constants.destPath + "example.xlsx");
    Style style = workbook.Worksheets[0].Cells["B12"].GetStyle();
    Assert.IsTrue(style.Font.IsBold);
    Assert.IsTrue(style.Font.IsStrikeout);
}
```

### See Also

* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


