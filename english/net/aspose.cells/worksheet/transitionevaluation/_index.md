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
// Called: Assert.IsTrue(workbook.Worksheets[0].TransitionEvaluation);
[Test]
        public void Property_TransitionEvaluation()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CELLSJAVA41429.xlsx");
            Assert.IsTrue(workbook.Worksheets[0].TransitionEvaluation);
            Assert.IsFalse(workbook.Worksheets[0].TransitionEntry);
            workbook.Save(Constants.destPath + "CELLSJAVA41429.xlsx");
            workbook = new Workbook(Constants.destPath + "CELLSJAVA41429.xlsx");
            Assert.IsTrue(workbook.Worksheets[0].TransitionEvaluation);
            Assert.IsFalse(workbook.Worksheets[0].TransitionEntry);
        }
```

### See Also

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


