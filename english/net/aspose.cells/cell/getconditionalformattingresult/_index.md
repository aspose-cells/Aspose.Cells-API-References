---
title: Cell.GetConditionalFormattingResult
second_title: Aspose.Cells for .NET API Reference
description: Cell method. Get the result of the conditional formatting
type: docs
url: /net/aspose.cells/cell/getconditionalformattingresult/
---
## Cell.GetConditionalFormattingResult method

Get the result of the conditional formatting.

```csharp
public ConditionalFormattingResult GetConditionalFormattingResult()
```

### Remarks

Returns null if no conditional formatting is applied to this cell,

### Examples

```csharp
// Called: ConditionalFormattingResult cfr = wb.Worksheets["Report"].Cells["L29"].GetConditionalFormattingResult();
[Test]
        public void Method_GetConditionalFormattingResult()
        {
            Workbook wb = new Workbook(Constants.sourcePath + "ConditionalFormattings/J42081_810858.xlsm");
            ConditionalFormattingResult cfr = wb.Worksheets["Report"].Cells["L29"].GetConditionalFormattingResult();
            Assert.AreEqual(0.95684885, cfr.ConditionalFormattingDataBar.MaxCfvo.Value, "DataBar.MaxValue");
        }
```

### See Also

* class [ConditionalFormattingResult](../../conditionalformattingresult/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


