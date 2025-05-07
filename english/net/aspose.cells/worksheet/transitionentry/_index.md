---
title: Worksheet.TransitionEntry
second_title: Aspose.Cells for .NET API Reference
description: Worksheet property. Indicates whether the Transition Formula Entry Lotus compatibility option is enabled
type: docs
url: /net/aspose.cells/worksheet/transitionentry/
---
## Worksheet.TransitionEntry property

Indicates whether the Transition Formula Entry (Lotus compatibility) option is enabled.

```csharp
public bool TransitionEntry { get; set; }
```

### Examples

```csharp
// Called: Assert.IsFalse(workbook.Worksheets[0].TransitionEntry);
[Test]
        public void Property_TransitionEntry()
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


