---
title: Font.IsSuperscript
second_title: Aspose.Cells for .NET API Reference
description: Font property. Gets or sets a value indicating whether the font is super script
type: docs
url: /net/aspose.cells/font/issuperscript/
---
## Font.IsSuperscript property

Gets or sets a value indicating whether the font is super script.

```csharp
public bool IsSuperscript { get; set; }
```

### Examples

```csharp
// Called: Assert.IsTrue(setting.Font.IsSuperscript);
public void Font_Property_IsSuperscript()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    Cell cell = workbook.Worksheets[0].Cells["A1"];
    FontSetting setting = cell.Characters(38, 1);
    Assert.IsTrue(setting.Font.IsSuperscript);
}
```

### See Also

* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


