---
title: SetBorderPosition
second_title: Référence de l'API Aspose.Cells pour .NET
description: Représente la position de la bordure à définir dune plage de cellules.
type: docs
weight: 900
url: /fr/net/aspose.cells.gridweb/setborderposition/
---
## SetBorderPosition enumeration

Représente la position de la bordure à définir d'une plage de cellules.

```csharp
public enum SetBorderPosition
```

### Valeurs

| Nom | Évaluer | La description |
| --- | --- | --- |
| Top | `0` | Bordure supérieure |
| Bottom | `1` | Bordure inférieure |
| Left | `2` | Bordure gauche |
| Right | `3` | Bord droit |
| HorizontalMiddle | `4` | Bordure inférieure |
| VerticalMiddle | `5` | Bordure médiane horizontale |
| Outline | `6` | Bordures centrales verticales |
| Cross | `7` | Transfrontalier |
| None | `8` | Aucune bordure |

### Exemples

```csharp
[C#]
	GridWeb1.WebWorksheets[0].Cells.SetBorders(0, 0, 5, 8, SetBorderPosition.Outline, borderStyle1);

[VB]
	GridWeb1.WebWorksheets(0).Cells.SetBorders(0, 0, 5, 8, SetBorderPosition.Outline, borderStyle1)
```

### Voir également

* espace de noms [Aspose.Cells.GridWeb](../../aspose.cells.gridweb)
* Assemblée [Aspose.Cells.GridWeb](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.GridWeb.dll -->
