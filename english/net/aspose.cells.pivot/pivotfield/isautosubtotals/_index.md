---
title: PivotField.IsAutoSubtotals
second_title: Aspose.Cells for .NET API Reference
description: PivotField property. Indicates whether the specified field shows automatic subtotals. Default is true
type: docs
url: /net/aspose.cells.pivot/pivotfield/isautosubtotals/
---
## PivotField.IsAutoSubtotals property

Indicates whether the specified field shows automatic subtotals. Default is true.

```csharp
public bool IsAutoSubtotals { get; set; }
```

### Examples

```csharp
// Called: pivotField.IsAutoSubtotals = subTotals;
private void PivotField_Property_IsAutoSubtotals(PivotTable pivotTable, string fieldName, string caption, bool subTotals = false)
        {
            PivotField pivotField = pivotTable.ColumnFields[pivotTable.AddFieldToArea(PivotFieldType.Column, fieldName)];
            pivotField.DisplayName = caption;
            pivotField.IsAutoSubtotals = subTotals;
            pivotField.IsAscendSort = true;
        }
```

### See Also

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


