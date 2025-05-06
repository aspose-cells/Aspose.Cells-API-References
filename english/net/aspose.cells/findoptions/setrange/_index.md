---
title: FindOptions.SetRange
second_title: Aspose.Cells for .NET API Reference
description: FindOptions method. Sets the searched range
type: docs
url: /net/aspose.cells/findoptions/setrange/
---
## FindOptions.SetRange method

Sets the searched range.

```csharp
public void SetRange(CellArea ca)
```

| Parameter | Type | Description |
| --- | --- | --- |
| ca | CellArea | the searched range. |

### Examples

```csharp
// Called: ContainsFindOptions.SetRange(cellarea);
private void Method_CellArea_(Workbook workbook)
        {
            Cells cells = workbook.Worksheets[0].Cells;
            CellArea cellarea = common.setCellArea(1, 1, 3, 3);
            ContainsFindOptions.CaseSensitive = true;
            ContainsFindOptions.SetRange(cellarea);
            Cell cell = cells.Find(&quot;ac&quot;, null, ContainsFindOptions);
            testAreEqual(null, cell, caseName);
        }
```

### See Also

* struct [CellArea](../../cellarea/)
* class [FindOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


