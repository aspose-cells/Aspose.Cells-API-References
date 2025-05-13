---
title: Style.IsLocked
second_title: Aspose.Cells for .NET API Reference
description: Style property. Gets or sets a value indicating whether a cell can be modified or not
type: docs
url: /net/aspose.cells/style/islocked/
---
## Style.IsLocked property

Gets or sets a value indicating whether a cell can be modified or not.

```csharp
public bool IsLocked { get; set; }
```

### Remarks

Locking cells has no effect unless the worksheet is protected.

### Examples

```csharp
// Called: testAreEqual(cellsSrc[10, 3].GetStyle().IsLocked, cellsDest[10, 3].GetStyle().IsLocked, caseName);
private void Style_Property_IsLocked(Workbook workbook)
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


