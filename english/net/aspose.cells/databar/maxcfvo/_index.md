---
title: DataBar.MaxCfvo
second_title: Aspose.Cells for .NET API Reference
description: DataBar property. Get or set this DataBars max value object. Cannot set null or CFValueObject with type FormatConditionValueType.Min to it
type: docs
url: /net/aspose.cells/databar/maxcfvo/
---
## DataBar.MaxCfvo property

Get or set this DataBar's max value object. Cannot set null or CFValueObject with type FormatConditionValueType.Min to it.

```csharp
public ConditionalFormattingValue MaxCfvo { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(0.95684885, cfr.ConditionalFormattingDataBar.MaxCfvo.Value, "DataBar.MaxValue");
public void DataBar_Property_MaxCfvo()
{
    Workbook wb = new Workbook(Constants.sourcePath + "example.xlsm");
    ConditionalFormattingResult cfr = wb.Worksheets["Report"].Cells["L29"].GetConditionalFormattingResult();
    Assert.AreEqual(0.95684885, cfr.ConditionalFormattingDataBar.MaxCfvo.Value, "DataBar.MaxValue");
}
```

### See Also

* class [ConditionalFormattingValue](../../conditionalformattingvalue/)
* class [DataBar](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


