---
title: FindOptions.SearchBackward
second_title: Aspose.Cells for .NET API Reference
description: FindOptions property. Whether search backward for cells
type: docs
url: /net/aspose.cells/findoptions/searchbackward/
---
## FindOptions.SearchBackward property

Whether search backward for cells.

```csharp
public bool SearchBackward { get; set; }
```

### Examples

```csharp
// Called: rangeOptions.SearchBackward = true;
private void Property_SearchBackward(Workbook workbook)
        {
            Cells cells = workbook.Worksheets[0].Cells;
            CellArea cellarea = common.setCellArea(1, 1, 3, 3);
            rangeOptions.SetRange(cellarea);
            rangeOptions.SearchBackward = true;
            Cell cell = cells.Find(&quot;abc&quot;, null, rangeOptions);
            testAreEqual(3, cell.Row, caseName);
            testAreEqual(1, cell.Column, caseName);
        }
```

### See Also

* class [FindOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


