---
title: "Énum SetBorderPosition"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Énum Aspose.Cells.GridWeb.SetBorderPosition. Représente la position de bordure à définir pour une plage de cellules."
type: docs
url: /fr/net/aspose.cells.gridweb/setborderposition/
---
## SetBorderPosition enumeration

Représente la position de la bordure à définir pour une plage de cellules.

```csharp
public enum SetBorderPosition
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Top | `0` | Bordure supérieure |
| Bottom | `1` | Bordure inférieure |
| Left | `2` | Bordure gauche |
| Right | `3` | Bordure droite |
| HorizontalMiddle | `4` | Bordure inférieure |
| VerticalMiddle | `5` | Bordures horizontales centrales |
| Outline | `6` | Bordures VerticalMiddle |
| Cross | `7` | Bordures croisées |
| None | `8` | Aucune bordure |

### Exemples

```csharp
[C#]
    GridWeb GridWeb1=new GridWeb();
	GridWeb1.WorkSheets[0].Cells.SetBorders(0, 0, 5, 8, SetBorderPosition.Outline, GridWeb1.WorkSheets[0].Cells[0, 0].Style.LeftBorderStyle);

[VB]
	GridWeb1.WorkSheets(0).Cells.SetBorders(0, 0, 5, 8, SetBorderPosition.Outline, GridWeb1.WorkSheets[0].Cells[0, 0].Style.LeftBorderStyle)
```

### Voir aussi

* namespace [Aspose.Cells.GridWeb](../../aspose.cells.gridweb/)
* assembly [Aspose.Cells.GridWeb](../../)


