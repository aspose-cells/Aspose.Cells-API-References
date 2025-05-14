---
title: ConditionalFormattingIcon.Type
second_title: Aspose.Cells for .NET API Reference
description: ConditionalFormattingIcon property. Gets and sets the icon set type
type: docs
url: /net/aspose.cells/conditionalformattingicon/type/
---
## ConditionalFormattingIcon.Type property

Gets and sets the icon set type.

```csharp
public IconSetType Type { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(formattingResult.ConditionalFormattingIcon.Type, IconSetType.Symbols32);
public void ConditionalFormattingIcon_Property_Type()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    Worksheet worksheet = workbook.Worksheets[0];

    workbook.CalculateFormula();

    Cell cell = worksheet.Cells["A2"];
    ConditionalFormattingResult formattingResult = cell.GetConditionalFormattingResult();
    Assert.AreEqual(formattingResult.ConditionalFormattingIcon.Type, IconSetType.Symbols32);
    Assert.AreEqual(formattingResult.ConditionalFormattingIcon.Index, 1);
}
```

### See Also

* enum [IconSetType](../../iconsettype/)
* class [ConditionalFormattingIcon](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


