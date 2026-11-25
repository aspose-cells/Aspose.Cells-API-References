---
title: "PivotField.Subtotals"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PivotField. Ottiene o imposta i subtotali del campo. Solo per campi pivot di tipo Riga o Colonna"
type: docs
url: /it/net/aspose.cells.pivot/pivotfield/subtotals/
---
## PivotField.Subtotals property

Ottiene o imposta i subtotali del campo. Solo per i campi pivot di riga o colonna.

```csharp
public PivotFieldSubtotalType Subtotals { get; set; }
```

### Esempi

```csharp

[C#]
//Nessun subtotale
rowField.Subtotals = PivotFieldSubtotalType.None;
//Subtotali automatici
//rowField.Subtotals = PivotFieldSubtotalType.Automatic;
//Subtotali singoli: Sum
//rowField.Subtotals = PivotFieldSubtotalType.Sum;
//Subtotali multipli: Sum e Count
//rowField.Subtotals = PivotFieldSubtotalType.Sum | PivotFieldSubtotalType.Count;
```

### Vedi anche

* enum [PivotFieldSubtotalType](../../pivotfieldsubtotaltype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


