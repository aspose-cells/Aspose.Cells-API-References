---
title: Style.IsFormulaHidden
second_title: Aspose.Cells for .NET API Reference
description: Style property. Represents if the formula will be hidden when the worksheet is protected
type: docs
url: /net/aspose.cells/style/isformulahidden/
---
## Style.IsFormulaHidden property

Represents if the formula will be hidden when the worksheet is protected.

```csharp
public bool IsFormulaHidden { get; set; }
```

### Examples

```csharp
// Called: testAreEqual(cellsSrc[10, 3].GetStyle().IsFormulaHidden, cellsDest[10, 3].GetStyle().IsFormulaHidden, caseName);
private void Style_Property_IsFormulaHidden(Workbook workbook)
        {
            Cells cellsSrc = workbook.Worksheets[0].Cells;
            Cells cellsDest = workbook.Worksheets["sheetDest"].Cells;
            testAreEqual(cellsSrc[3, 2].GetStyle().IsLocked, cellsDest[3, 2].GetStyle().IsLocked, caseName);
            testAreEqual(cellsSrc[3, 2].GetStyle().IsFormulaHidden, cellsDest[3, 2].GetStyle().IsFormulaHidden, caseName);
            testAreEqual(cellsSrc[4, 5].GetStyle().IsLocked, cellsDest[4, 5].GetStyle().IsLocked, caseName);
            testAreEqual(cellsSrc[4, 5].GetStyle().IsFormulaHidden, cellsDest[4, 5].GetStyle().IsFormulaHidden, caseName);
            testAreEqual(cellsSrc[10, 3].GetStyle().IsLocked, cellsDest[10, 3].GetStyle().IsLocked, caseName);
            testAreEqual(cellsSrc[10, 3].GetStyle().IsFormulaHidden, cellsDest[10, 3].GetStyle().IsFormulaHidden, caseName);
            testAreEqual(cellsSrc[13, 7].GetStyle().IsLocked, cellsDest[13, 7].GetStyle().IsLocked, caseName);
            testAreEqual(cellsSrc[13, 7].GetStyle().IsFormulaHidden, cellsDest[13, 7].GetStyle().IsFormulaHidden, caseName);
        }
```

### See Also

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


