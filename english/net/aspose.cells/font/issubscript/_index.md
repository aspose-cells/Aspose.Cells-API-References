---
title: Font.IsSubscript
second_title: Aspose.Cells for .NET API Reference
description: Font property. Gets or sets a value indicating whether the font is subscript
type: docs
url: /net/aspose.cells/font/issubscript/
---
## Font.IsSubscript property

Gets or sets a value indicating whether the font is subscript.

```csharp
public bool IsSubscript { get; set; }
```

### Examples

```csharp
// Called: Assert.IsTrue(style.Font.IsSubscript);
public void Font_Property_IsSubscript()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.ods");
    Style style = workbook.Worksheets[0].Cells["A8"].GetStyle();
    Assert.IsTrue(style.Font.IsSubscript);
    Assert.IsFalse(style.Font.IsSuperscript);
    style = workbook.Worksheets[0].Cells["A9"].GetStyle();
    Assert.IsFalse(style.Font.IsSubscript);
    Assert.IsTrue(style.Font.IsSuperscript);
    workbook.Save(Constants.destPath + "example.ods");
    workbook = new Workbook(Constants.destPath + "example.ods");
    style = workbook.Worksheets[0].Cells["A8"].GetStyle();
    Assert.IsTrue(style.Font.IsSubscript);
    Assert.IsFalse(style.Font.IsSuperscript);
    style = workbook.Worksheets[0].Cells["A9"].GetStyle();
    Assert.IsFalse(style.Font.IsSubscript);
    Assert.IsTrue(style.Font.IsSuperscript);
}
```

### See Also

* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


