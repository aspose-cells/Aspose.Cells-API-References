---
title: ConditionalFormattingResult.ConditionalFormattingDataBar
second_title: Aspose.Cells for .NET API Reference
description: ConditionalFormattingResult property. Gets the DataBar object
type: docs
url: /net/aspose.cells/conditionalformattingresult/conditionalformattingdatabar/
---
## ConditionalFormattingResult.ConditionalFormattingDataBar property

Gets the DataBar object.

```csharp
public DataBar ConditionalFormattingDataBar { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual((double)(formattingResult.ConditionalFormattingDataBar.MinCfvo.Value), -150);
[Test]
        public void Property_ConditionalFormattingDataBar()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;ConditionalFormattings/CELLSNET-42116.xlsx&quot;);
            Worksheet worksheet = workbook.Worksheets[0];

            workbook.CalculateFormula();

            Cell cell = worksheet.Cells[&quot;A1&quot;];
            ConditionalFormattingResult formattingResult = cell.GetConditionalFormattingResult();
            Assert.AreEqual((double)(formattingResult.ConditionalFormattingDataBar.MinCfvo.Value), -6);
            cell = worksheet.Cells[&quot;D10&quot;];
            formattingResult = cell.GetConditionalFormattingResult();
            Assert.AreEqual((double)(formattingResult.ConditionalFormattingDataBar.MinCfvo.Value), -5);
            Assert.AreEqual((double)(formattingResult.ConditionalFormattingDataBar.MaxCfvo.Value), -1);
            cell = worksheet.Cells[&quot;H2&quot;];
            formattingResult = cell.GetConditionalFormattingResult();
            Assert.AreEqual((double)(formattingResult.ConditionalFormattingDataBar.MinCfvo.Value), -150);
            Assert.AreEqual((double)(formattingResult.ConditionalFormattingDataBar.MaxCfvo.Value), 100);
            cell = worksheet.Cells[&quot;G10&quot;];
            formattingResult = cell.GetConditionalFormattingResult();
            Assert.AreEqual((double)(formattingResult.ConditionalFormattingDataBar.MinCfvo.Value), -1);
            Assert.AreEqual((double)(formattingResult.ConditionalFormattingDataBar.MaxCfvo.Value), -1);

        }
```

### See Also

* class [DataBar](../../databar/)
* class [ConditionalFormattingResult](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


