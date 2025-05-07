---
title: PivotField.DisplayName
second_title: Aspose.Cells for .NET API Reference
description: PivotField property. Represents the PivotField display name
type: docs
url: /net/aspose.cells.pivot/pivotfield/displayname/
---
## PivotField.DisplayName property

Represents the PivotField display name.

```csharp
public string DisplayName { get; set; }
```

### Examples

```csharp
// Called: pivotField.DisplayName = caption;
private void Property_DisplayName(PivotTable pivotTable, string fieldName, string caption, bool subTotals = false)
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


