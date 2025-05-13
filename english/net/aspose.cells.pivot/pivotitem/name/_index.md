---
title: PivotItem.Name
second_title: Aspose.Cells for .NET API Reference
description: PivotItem property. Gets the name of the pivot item
type: docs
url: /net/aspose.cells.pivot/pivotitem/name/
---
## PivotItem.Name property

Gets the name of the pivot item.

```csharp
public string Name { get; set; }
```

### Examples

```csharp
// Called: item.IsHidden = item.Name != "债券借贷";
public void PivotItem_Property_Name()
{
    Workbook wb = new Workbook(Constants.PivotTableSourcePath + "example.xlsx");
    var worksheet = wb.Worksheets[0];
    var pivotTable = worksheet.PivotTables[0];
    var field = pivotTable.ColumnFields[1];

    foreach (PivotItem item in field.PivotItems)
    {
        item.IsHidden = item.Name != "债券借贷";
    }

    // 抛出错误 Aspose.Cells.CellsException:“Cells in range D2:D3 cannot be merged because cells in range B2:H2 have already been merged.”
    worksheet.RefreshPivotTables();
    Assert.AreEqual(2, worksheet.Cells.GetMergedAreas().Length);
    Assert.IsFalse(worksheet.Cells["B2"].IsMerged);
    Assert.IsTrue(worksheet.Cells["D2"].IsMerged);
    wb.Save(Constants.PivotTableDestPath + "example.xlsx");
}
```

### See Also

* class [PivotItem](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


