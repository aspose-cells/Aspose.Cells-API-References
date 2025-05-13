---
title: PivotField.NonAutoSortDefault
second_title: Aspose.Cells for .NET API Reference
description: PivotField property. Indicates whether a sort operation that will be applied to this pivot field is an autosort operation or a simple data sort
type: docs
url: /net/aspose.cells.pivot/pivotfield/nonautosortdefault/
---
## PivotField.NonAutoSortDefault property

Indicates whether a sort operation that will be applied to this pivot field is an autosort operation or a simple data sort.

```csharp
public bool NonAutoSortDefault { get; set; }
```

### Examples

```csharp
// Called: Assert.IsTrue(pivotField.NonAutoSortDefault);
public void PivotField_Property_NonAutoSortDefault()
{
    PivotField pivotField = null;
    Workbook workbook = new Workbook(Constants.PivotTableSourcePath + "example.xlsx");           
    pivotField = workbook.Worksheets[0].PivotTables[0].RowFields[0];
    Assert.IsTrue(pivotField.NonAutoSortDefault);
    workbook = Util.ReSave(workbook, SaveFormat.Xlsb);
    pivotField = workbook.Worksheets[0].PivotTables[0].RowFields[0];
    Assert.IsTrue(pivotField.NonAutoSortDefault);
    workbook = Util.ReSave(workbook, SaveFormat.Xlsx);
    pivotField = workbook.Worksheets[0].PivotTables[0].RowFields[0];
    Assert.IsTrue(pivotField.NonAutoSortDefault);
}
```

### See Also

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


