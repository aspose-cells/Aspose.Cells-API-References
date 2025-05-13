---
title: PivotField.Ungroup
second_title: Aspose.Cells for .NET API Reference
description: PivotField method. Ungroup the pivot field
type: docs
url: /net/aspose.cells.pivot/pivotfield/ungroup/
---
## PivotField.Ungroup method

Ungroup the pivot field.

```csharp
public void Ungroup()
```

### Examples

```csharp
// Called: pt.ColumnFields[0].Ungroup();
public void PivotField_Method_Ungroup()
{
    Workbook workbook = new Workbook(Constants.PivotTableSourcePath + "example.xlsx");
    PivotTable pt = workbook.Worksheets[0].PivotTables[0];
    pt.ColumnFields[0].Ungroup();
    Assert.AreEqual(1, pt.ColumnFields.Count);
    Assert.AreEqual("1", workbook.Worksheets[0].Cells["H8"].StringValue);

    workbook.Save(Constants.PIVOT_CHECK_FILE_PATH + "example.xlsx");

}
```

### See Also

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


