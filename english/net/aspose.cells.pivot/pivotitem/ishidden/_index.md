---
title: PivotItem.IsHidden
second_title: Aspose.Cells for .NET API Reference
description: PivotItem property. Gets and Sets whether the pivot item is hidden
type: docs
url: /net/aspose.cells.pivot/pivotitem/ishidden/
---
## PivotItem.IsHidden property

Gets and Sets whether the pivot item is hidden.

```csharp
public bool IsHidden { get; set; }
```

### Examples

```csharp
// Called: item.IsHidden = item.Name != "债券借贷";
public void PivotItem_Property_IsHidden()
{
    var wb = new Workbook(Constants.PivotTableSourcePath + "example.xlsx");
    var worksheet = wb.Worksheets[0];
    var pivotTable = worksheet.PivotTables[0];
    var field = pivotTable.ColumnFields[1];

    foreach (PivotItem item in field.PivotItems)
    {
        item.IsHidden = item.Name != "债券借贷";
    }

    // Aspose.Cells.CellsException:“Cells in range D2:D3 cannot be merged because cells in range B2:H2 have already been merged.”
    worksheet.RefreshPivotTables();
}
```

### See Also

* class [PivotItem](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


