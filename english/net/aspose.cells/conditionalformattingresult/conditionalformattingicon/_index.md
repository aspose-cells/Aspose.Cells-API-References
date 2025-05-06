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
// Called: Assert.AreEqual(formattingResult.ConditionalFormattingIcon.Index, 1);
[Test]
        public void Property_ConditionalFormattingIcon()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;ConditionalFormattings/CELLSNET-42119.xlsx&quot;);
            Worksheet worksheet = workbook.Worksheets[0];

            workbook.CalculateFormula();

            Cell cell = worksheet.Cells[&quot;A2&quot;];
            ConditionalFormattingResult formattingResult = cell.GetConditionalFormattingResult();
            Assert.AreEqual(formattingResult.ConditionalFormattingIcon.Type, IconSetType.Symbols32);
            Assert.AreEqual(formattingResult.ConditionalFormattingIcon.Index, 1);
        }
```

### See Also

* class [ConditionalFormattingIcon](../../conditionalformattingicon/)
* class [ConditionalFormattingResult](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


