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
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CELLSJAVA41429.xlsx&quot;);
            Assert.IsTrue(workbook.Worksheets[0].TransitionEvaluation);
            Assert.IsFalse(workbook.Worksheets[0].TransitionEntry);
            workbook.Save(Constants.destPath + &quot;CELLSJAVA41429.xlsx&quot;);
            workbook = new Workbook(Constants.destPath + &quot;CELLSJAVA41429.xlsx&quot;);
            Assert.IsTrue(workbook.Worksheets[0].TransitionEvaluation);
            Assert.IsFalse(workbook.Worksheets[0].TransitionEntry);
        }
```

### See Also

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


