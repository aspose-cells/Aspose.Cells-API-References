---
title: ConditionalFormattingResult.ConditionalStyle
second_title: Aspose.Cells for .NET API Reference
description: ConditionalFormattingResult property. Gets the conditional result style
type: docs
url: /net/aspose.cells/conditionalformattingresult/conditionalstyle/
---
## ConditionalFormattingResult.ConditionalStyle property

Gets the conditional result style.

```csharp
public Style ConditionalStyle { get; }
```

### Examples

```csharp
// Called: Style style = cell.GetConditionalFormattingResult().ConditionalStyle;
public void ConditionalFormattingResult_Property_ConditionalStyle()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "ConditionalFormattings/ConditionalTest_4.8.2.2.xlsx");
    Cell cell = workbook.Worksheets[0].Cells["B2"];
    Style style = cell.GetConditionalFormattingResult().ConditionalStyle;
    Assert.AreEqual(style.Font.Color.ToArgb() & 0xFFFFFF, Color.Red.ToArgb() & 0xFFFFFF);
}
```

### See Also

* class [Style](../../style/)
* class [ConditionalFormattingResult](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


