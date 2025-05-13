---
title: PivotField.IsCalculatedField
second_title: Aspose.Cells for .NET API Reference
description: PivotField property. Indicates whether the specified PivotTable field is calculated field
type: docs
url: /net/aspose.cells.pivot/pivotfield/iscalculatedfield/
---
## PivotField.IsCalculatedField property

Indicates whether the specified PivotTable field is calculated field.

```csharp
public bool IsCalculatedField { get; }
```

### Examples

```csharp
// Called: Assert.IsTrue(pt.BaseFields[4].IsCalculatedField);
public void PivotField_Property_IsCalculatedField()
{
    Workbook workbook = new Workbook(Constants.PivotTableSourcePath + "example.xls");
    PivotTable pt = workbook.Worksheets[0].PivotTables[0];
    Assert.IsTrue(pt.BaseFields[4].IsCalculatedField);
   // Assert.IsTrue(pt.BaseFields[5].IsGroupField);
    workbook.Save(Constants.PivotTableDestPath + "example.xls");
    workbook = new Workbook(Constants.PivotTableDestPath + "example.xls");
     pt = workbook.Worksheets[0].PivotTables[0];
    Assert.IsTrue(pt.BaseFields[4].IsCalculatedField);
  //  Assert.IsTrue(pt.BaseFields[5].IsGroupField);
   // Assert.IsTrue(pt.BaseFields[1].IsGroupField);
}
```

### See Also

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


