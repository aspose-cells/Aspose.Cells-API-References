---
title: Worksheet.TransitionEvaluation
second_title: Aspose.Cells for .NET API Reference
description: Worksheet property. Indicates whether the Transition Formula Evaluation Lotus compatibility option is enabled
type: docs
url: /net/aspose.cells/worksheet/transitionevaluation/
---
## Worksheet.TransitionEvaluation property

Indicates whether the Transition Formula Evaluation (Lotus compatibility) option is enabled.

```csharp
public bool TransitionEvaluation { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(workbook.Worksheets[0].TransitionEvaluation,true);
[Test]
        public void Property_TransitionEvaluation()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            workbook.Worksheets[0].TransitionEvaluation = true;
            cells[&quot;A1&quot;].PutValue(3);
            cells[&quot;A2&quot;].PutValue(&quot;test&quot;);
            cells[&quot;A3&quot;].PutValue(5);
            cells[&quot;B1&quot;].Formula = &quot;=A1+A2+A3&quot;;
            workbook.CalculateFormula();
            
            Assert.AreEqual(cells[&quot;B1&quot;].DoubleValue, 8);
            workbook = Util.ReSave(workbook, SaveFormat.Excel97To2003);
            Assert.AreEqual(workbook.Worksheets[0].TransitionEvaluation,true);
            workbook.Worksheets[0].TransitionEvaluation = false;
            workbook.CalculateFormula();
            Assert.AreEqual(workbook.Worksheets[0].Cells[&quot;B1&quot;].StringValue, &quot;#VALUE!&quot;);
        }
```

### See Also

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


