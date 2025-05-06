---
title: ConditionalFormattingValue.Value
second_title: Aspose.Cells for .NET API Reference
description: ConditionalFormattingValue property. Get or set the value of this conditional formatting value object. It should be used in conjunction with Type
type: docs
url: /net/aspose.cells/conditionalformattingvalue/value/
---
## ConditionalFormattingValue.Value property

Get or set the value of this conditional formatting value object. It should be used in conjunction with Type.

```csharp
public object Value { get; set; }
```

### Remarks

If the value is string and start with "=", it will be processed as a formula, otherwise we will process it as a simple value.

### Examples

```csharp
// Called: Assert.AreEqual(0.95684885, cfr.ConditionalFormattingDataBar.MaxCfvo.Value, &amp;quot;DataBar.MaxValue&amp;quot;);
[Test]
        public void Property_Value()
        {
            Workbook wb = new Workbook(Constants.sourcePath + &quot;ConditionalFormattings/J42081_810858.xlsm&quot;);
            ConditionalFormattingResult cfr = wb.Worksheets[&quot;Report&quot;].Cells[&quot;L29&quot;].GetConditionalFormattingResult();
            Assert.AreEqual(0.95684885, cfr.ConditionalFormattingDataBar.MaxCfvo.Value, &quot;DataBar.MaxValue&quot;);
        }
```

### See Also

* class [ConditionalFormattingValue](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


