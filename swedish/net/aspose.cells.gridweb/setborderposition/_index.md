---
title: "Enum SetBorderPosition"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.GridWeb.SetBorderPosition-enum. Representerar kantpositionen som ska sättas för ett cellområde"
type: docs
url: /sv/net/aspose.cells.gridweb/setborderposition/
---
## SetBorderPosition enumeration

Representerar kantpositionen som ska sättas för ett cellområde.

```csharp
public enum SetBorderPosition
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Top | `0` | Övre kant |
| Bottom | `1` | Nedre kant |
| Left | `2` | Vänster kant |
| Right | `3` | Höger kant |
| HorizontalMiddle | `4` | Nedre kant |
| VerticalMiddle | `5` | Horisontella mittenkanter |
| Outline | `6` | Vertikala mittenkanter |
| Cross | `7` | Korskanter |
| None | `8` | Inga kanter |

### Exempel

```csharp
[C#]
    GridWeb GridWeb1=new GridWeb();
	GridWeb1.WorkSheets[0].Cells.SetBorders(0, 0, 5, 8, SetBorderPosition.Outline, GridWeb1.WorkSheets[0].Cells[0, 0].Style.LeftBorderStyle);

[VB]
	GridWeb1.WorkSheets(0).Cells.SetBorders(0, 0, 5, 8, SetBorderPosition.Outline, GridWeb1.WorkSheets[0].Cells[0, 0].Style.LeftBorderStyle)
```

### Se även

* namespace [Aspose.Cells.GridWeb](../../aspose.cells.gridweb/)
* assembly [Aspose.Cells.GridWeb](../../)


