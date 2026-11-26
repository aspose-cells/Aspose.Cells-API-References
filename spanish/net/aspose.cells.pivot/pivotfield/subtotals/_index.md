---
title: "PivotField.Subtotals"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PivotField. Obtiene o establece los subtotales del campo. Sólo para campos dinámicos de fila o columna"
type: docs
url: /es/net/aspose.cells.pivot/pivotfield/subtotals/
---
## PivotField.Subtotals property

Obtiene o establece los subtotales del campo. Solo para campos dinámicos de fila o columna.

```csharp
public PivotFieldSubtotalType Subtotals { get; set; }
```

### Ejemplos

```csharp

[C#]
//Sin subtotales
rowField.Subtotals = PivotFieldSubtotalType.None;
//Subtotales automáticos
//rowField.Subtotals = PivotFieldSubtotalType.Automatic;
//Subtotales simples: Sum
//rowField.Subtotals = PivotFieldSubtotalType.Sum;
//Subtotales múltiples: Sum y count numbers 
//rowField.Subtotals = PivotFieldSubtotalType.Sum | PivotFieldSubtotalType.Count;
```

### Ver también

* enum [PivotFieldSubtotalType](../../pivotfieldsubtotaltype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


