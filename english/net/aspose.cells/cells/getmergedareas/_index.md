---
title: Cells.GetMergedAreas
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Gets all merged cells
type: docs
url: /net/aspose.cells/cells/getmergedareas/
---
## Cells.GetMergedAreas method

Gets all merged cells.

```csharp
public CellArea[] GetMergedAreas()
```

### Examples

```csharp
// Called: testAreEqual(1, cells.GetMergedAreas().Length, caseName);
private void Method_GetMergedAreas(Workbook workbook)
        {
            Cells cells = workbook.Worksheets[0].Cells;
            testAreEqual(1, cells.GetMergedAreas().Length, caseName);
        }
```

### See Also

* struct [CellArea](../../cellarea/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


