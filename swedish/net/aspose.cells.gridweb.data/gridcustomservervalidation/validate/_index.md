---
title: "GridCustomServerValidation.Validate"
second_title: "Aspose.Cells för .NET API‑referens"
description: "GridCustomServerValidation metod."
type: docs
url: /sv/net/aspose.cells.gridweb.data/gridcustomservervalidation/validate/
---
## GridCustomServerValidation.Validate method

```csharp
public string Validate(GridWorksheet sheet, int row, int col, string value)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| blad | GridWorksheet | GridWorksheet |
| row | Int32 | radindex för cellen |
| kol | Int32 | kolumnindex för cellen |
| värde | String | värdet för validering |

### Returvärde

strängbaserat resultatvärde

### Anmärkningar

Om du returnerar string.empty anses valideringen godkänd, annars kan du returnera ett relaterat meddelande som kan hanteras i ClientCallback-funktionen.

### Se även

* class [GridWorksheet](../../gridworksheet/)
* interface [GridCustomServerValidation](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)


