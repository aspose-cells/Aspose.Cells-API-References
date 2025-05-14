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
// Called: Assert.AreEqual((double)(formattingResult.ConditionalFormattingDataBar.MinCfvo.Value), -6);
public void ConditionalFormattingResult_Property_ConditionalFormattingDataBar()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    Worksheet worksheet = workbook.Worksheets[0];

    workbook.CalculateFormula();

    Cell cell = worksheet.Cells["A1"];
    ConditionalFormattingResult formattingResult = cell.GetConditionalFormattingResult();
    Assert.AreEqual((double)(formattingResult.ConditionalFormattingDataBar.MinCfvo.Value), -6);
    cell = worksheet.Cells["D10"];
    formattingResult = cell.GetConditionalFormattingResult();
    Assert.AreEqual((double)(formattingResult.ConditionalFormattingDataBar.MinCfvo.Value), -5);
    Assert.AreEqual((double)(formattingResult.ConditionalFormattingDataBar.MaxCfvo.Value), -1);
    cell = worksheet.Cells["H2"];
    formattingResult = cell.GetConditionalFormattingResult();
    Assert.AreEqual((double)(formattingResult.ConditionalFormattingDataBar.MinCfvo.Value), -150);
    Assert.AreEqual((double)(formattingResult.ConditionalFormattingDataBar.MaxCfvo.Value), 100);
    cell = worksheet.Cells["G10"];
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


