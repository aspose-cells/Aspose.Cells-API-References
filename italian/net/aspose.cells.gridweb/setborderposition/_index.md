---
title: "Enum SetBorderPosition"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Enum Aspose.Cells.GridWeb.SetBorderPosition. Rappresenta la posizione del bordo da impostare per un intervallo di celle"
type: docs
url: /it/net/aspose.cells.gridweb/setborderposition/
---
## SetBorderPosition enumeration

Rappresenta la posizione del bordo da impostare per un intervallo di celle.

```csharp
public enum SetBorderPosition
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Top | `0` | Bordo superiore |
| Bottom | `1` | Bordo inferiore |
| Left | `2` | Bordo sinistro |
| Right | `3` | Bordo destro |
| HorizontalMiddle | `4` | Bordo inferiore |
| VerticalMiddle | `5` | Bordi orizzontali centrali |
| Outline | `6` | Bordi VerticalMiddle |
| Cross | `7` | Bordi incrociati |
| None | `8` | Nessun bordo |

### Esempi

```csharp
[C#]
    GridWeb GridWeb1=new GridWeb();
	GridWeb1.WorkSheets[0].Cells.SetBorders(0, 0, 5, 8, SetBorderPosition.Outline, GridWeb1.WorkSheets[0].Cells[0, 0].Style.LeftBorderStyle);

[VB]
	GridWeb1.WorkSheets(0).Cells.SetBorders(0, 0, 5, 8, SetBorderPosition.Outline, GridWeb1.WorkSheets[0].Cells[0, 0].Style.LeftBorderStyle)
```

### Vedi anche

* namespace [Aspose.Cells.GridWeb](../../aspose.cells.gridweb/)
* assembly [Aspose.Cells.GridWeb](../../)


