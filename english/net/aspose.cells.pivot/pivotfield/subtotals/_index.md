---
title: PivotField.Subtotals
second_title: Aspose.Cells for .NET API Reference
description: PivotField property. Gets or sets the subtotals of the field. Only for Row or Column pivot field
type: docs
url: /net/aspose.cells.pivot/pivotfield/subtotals/
---
## PivotField.Subtotals property

Gets or sets the subtotals of the field. Only for Row or Column pivot field.

```csharp
public PivotFieldSubtotalType Subtotals { get; set; }
```

### Examples

```csharp

[C#]
//No subtotals
rowField.Subtotals = PivotFieldSubtotalType.None;
//Automatic subtotals
//rowField.Subtotals = PivotFieldSubtotalType.Automatic;
//Single subtotals: Sum
//rowField.Subtotals = PivotFieldSubtotalType.Sum;
//Multipl subtotals: Sum and count numbers 
//rowField.Subtotals = PivotFieldSubtotalType.Sum | PivotFieldSubtotalType.Count;
```

### See Also

* enum [PivotFieldSubtotalType](../../pivotfieldsubtotaltype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


