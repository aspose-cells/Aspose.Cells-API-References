---
title: ConditionalFormattingResult.ConditionalFormattingIcon
second_title: Aspose.Cells for .NET API Reference
description: ConditionalFormattingResult property. Gets the image of icon set
type: docs
url: /net/aspose.cells/conditionalformattingresult/conditionalformattingicon/
---
## ConditionalFormattingResult.ConditionalFormattingIcon property

Gets the image of icon set.

```csharp
public ConditionalFormattingIcon ConditionalFormattingIcon { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(formattingResult == null || formattingResult.ConditionalFormattingIcon == null,true);
public void ConditionalFormattingResult_Property_ConditionalFormattingIcon()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    Worksheet worksheet = workbook.Worksheets[0];

    workbook.CalculateFormula();

    Cell cell = worksheet.Cells["A1"];
    ConditionalFormattingResult formattingResult = cell.GetConditionalFormattingResult();

    Assert.AreEqual(formattingResult == null || formattingResult.ConditionalFormattingIcon == null,true);
}
```

### See Also

* class [ConditionalFormattingIcon](../../conditionalformattingicon/)
* class [ConditionalFormattingResult](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


