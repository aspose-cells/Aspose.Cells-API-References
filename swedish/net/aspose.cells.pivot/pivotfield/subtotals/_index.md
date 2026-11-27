---
title: "PivotField.Subtotals"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotField-egenskap. Hämtar eller anger delsummerna för fältet. Endast för rad- eller kolumnpivottfält"
type: docs
url: /sv/net/aspose.cells.pivot/pivotfield/subtotals/
---
## PivotField.Subtotals property

Hämtar eller anger delsummerna för fältet. Endast för rad- eller kolumnpivotfält.

```csharp
public PivotFieldSubtotalType Subtotals { get; set; }
```

### Exempel

```csharp

[C#]
//Inga delsummer
rowField.Subtotals = PivotFieldSubtotalType.None;
//Automatiska delsummer
//rowField.Subtotals = PivotFieldSubtotalType.Automatic;
//Enkel delsummer: Sum
//rowField.Subtotals = PivotFieldSubtotalType.Sum;
//Multipla delsummer: Sum och räkna antal
//rowField.Subtotals = PivotFieldSubtotalType.Sum | PivotFieldSubtotalType.Count;
```

### Se även

* enum [PivotFieldSubtotalType](../../pivotfieldsubtotaltype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


