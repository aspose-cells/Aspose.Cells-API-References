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
// Called: r = sheet1.Cells[&amp;quot;E2&amp;quot;].GetConditionalFormattingResult();
[Test]
        public void Method_GetConditionalFormattingResult()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;ConditionalFormattings/TestConditionalIcon1.xlsx&quot;);
            Worksheet sheet1 = workbook.Worksheets[0];
            ConditionalFormattingResult r = sheet1.Cells[&quot;C2&quot;].GetConditionalFormattingResult();
            Assert.AreEqual(r.ConditionalFormattingIcon.Index, 2);
            r = sheet1.Cells[&quot;D2&quot;].GetConditionalFormattingResult();
            Assert.AreEqual(r.ConditionalFormattingIcon.Index, 1);
            r = sheet1.Cells[&quot;E2&quot;].GetConditionalFormattingResult();
            Assert.AreEqual(r.ConditionalFormattingIcon.Index, 0);
            FormatConditionCollection conditionCollection = sheet1.ConditionalFormattings[0];
            FormatCondition condition = conditionCollection[0];
        
            ConditionalFormattingIconCollection iconCollection = condition.IconSet.CfIcons;
            Assert.AreEqual(0, iconCollection[0].Index);
            Assert.AreEqual(1, iconCollection[1].Index);
            Assert.AreEqual(2, iconCollection[2].Index);

        }
```

### See Also

* class [ConditionalFormattingResult](../../conditionalformattingresult/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


