---
title: "PivotField.Subtotals"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotField-Eigenschaft. Gibt die Zwischensummen des Feldes zurück oder legt sie fest. Nur für Zeilen- oder Spalten-Pivot-Feld."
type: docs
url: /de/net/aspose.cells.pivot/pivotfield/subtotals/
---
## PivotField.Subtotals property

Liest oder legt die Zwischensummen des Feldes fest. Nur für Zeilen‑ oder Spalten‑Pivot‑Feld.

```csharp
public PivotFieldSubtotalType Subtotals { get; set; }
```

### Beispiele

```csharp

[C#]
//Keine Zwischensummen
rowField.Subtotals = PivotFieldSubtotalType.None;
//Automatische Zwischensummen
//rowField.Subtotals = PivotFieldSubtotalType.Automatic;
//Einzelne Zwischensummen: Summe
//rowField.Subtotals = PivotFieldSubtotalType.Sum;
//Mehrfache Zwischensummen: Summe und Anzahl der Zahlen
//rowField.Subtotals = PivotFieldSubtotalType.Sum | PivotFieldSubtotalType.Count;
```

### Siehe auch

* enum [PivotFieldSubtotalType](../../pivotfieldsubtotaltype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


