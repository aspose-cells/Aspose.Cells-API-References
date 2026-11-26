---
title: "Enumeración SetBorderPosition"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.GridWeb.SetBorderPosition enumeración. Representa la posición del borde que se establecerá en un rango de celdas."
type: docs
url: /es/net/aspose.cells.gridweb/setborderposition/
---
## SetBorderPosition enumeration

Representa la posición del borde que se debe establecer para un rango de celdas.

```csharp
public enum SetBorderPosition
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Top | `0` | Borde superior |
| Bottom | `1` | Borde inferior |
| Left | `2` | Borde izquierdo |
| Right | `3` | Borde derecho |
| HorizontalMiddle | `4` | Borde inferior |
| VerticalMiddle | `5` | Bordes horizontales medios |
| Outline | `6` | bordes VerticalMiddle |
| Cross | `7` | bordes cruzados |
| None | `8` | Sin bordes |

### Ejemplos

```csharp
[C#]
    GridWeb GridWeb1=new GridWeb();
	GridWeb1.WorkSheets[0].Cells.SetBorders(0, 0, 5, 8, SetBorderPosition.Outline, GridWeb1.WorkSheets[0].Cells[0, 0].Style.LeftBorderStyle);

[VB]
	GridWeb1.WorkSheets(0).Cells.SetBorders(0, 0, 5, 8, SetBorderPosition.Outline, GridWeb1.WorkSheets[0].Cells[0, 0].Style.LeftBorderStyle)
```

### Ver también

* namespace [Aspose.Cells.GridWeb](../../aspose.cells.gridweb/)
* assembly [Aspose.Cells.GridWeb](../../)


