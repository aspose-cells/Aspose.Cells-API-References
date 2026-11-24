---
title: "Enum SetBorderPosition"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.GridWeb.SetBorderPosition enum. Stellt die zu setzende Randposition eines Zellenbereichs dar."
type: docs
url: /de/net/aspose.cells.gridweb/setborderposition/
---
## SetBorderPosition enumeration

Stellt die Randposition dar, die für einen Zellenbereich festgelegt werden soll.

```csharp
public enum SetBorderPosition
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| Top | `0` | Oberer Rand |
| Bottom | `1` | Unterer Rand |
| Left | `2` | Linker Rand |
| Right | `3` | Rechter Rand |
| HorizontalMiddle | `4` | Unterer Rand |
| VerticalMiddle | `5` | Horizontale Mittelränder |
| Outline | `6` | Vertikale Mittelränder |
| Cross | `7` | Kreuzränder |
| None | `8` | Keine Ränder |

### Beispiele

```csharp
[C#]
    GridWeb GridWeb1=new GridWeb();
	GridWeb1.WorkSheets[0].Cells.SetBorders(0, 0, 5, 8, SetBorderPosition.Outline, GridWeb1.WorkSheets[0].Cells[0, 0].Style.LeftBorderStyle);

[VB]
	GridWeb1.WorkSheets(0).Cells.SetBorders(0, 0, 5, 8, SetBorderPosition.Outline, GridWeb1.WorkSheets[0].Cells[0, 0].Style.LeftBorderStyle)
```

### Siehe auch

* namespace [Aspose.Cells.GridWeb](../../aspose.cells.gridweb/)
* assembly [Aspose.Cells.GridWeb](../../)


