---
title: CreateValidation
second_title: Aspose.Cells for .NET API Reference
description: Creates a validation object for a cell.
type: docs
weight: 210
url: /net/aspose.cells.gridweb.data/gridcell/createvalidation/
---
## GridCell.CreateValidation method

Creates a validation object for a cell.

```csharp
public GridValidation CreateValidation(GridValidationType validationType, bool isRequried)
```

| Parameter | Type | Description |
| --- | --- | --- |
| validationType | GridValidationType | Validation type. |
| isRequried | Boolean | Whether the cell value is required. |

### Examples

```csharp
[C#]
	Validation v = cell1.CreateValidation(GridValidationType.CustomExpression, true);
	// Sets to number validation expression.
	v.RegEx = "\\d+";
	
[Visual Basic]
	Dim v As Validation =  cell1.CreateValidation(GridValidationType.CustomExpression,True) 
	 ' Sets to number validation expression.
	v.RegEx = "\\d+"
```

### See Also

* class [GridValidation](../../gridvalidation)
* enum [GridValidationType](../../gridvalidationtype)
* class [GridCell](../../gridcell)
* namespace [Aspose.Cells.GridWeb.Data](../../gridcell)
* assembly [Aspose.Cells.GridWeb](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.GridWeb.dll -->
