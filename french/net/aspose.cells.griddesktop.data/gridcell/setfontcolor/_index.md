---
title: SetFontColor
second_title: Référence de l'API Aspose.Cells pour .NET
description: Définit la couleur de la police sur la cellule. Pour améliorer les performances implémentez la méthode SetFontColor nimplémentez pas la propriété FontColor.
type: docs
weight: 390
url: /fr/net/aspose.cells.griddesktop.data/gridcell/setfontcolor/
---
## GridCell.SetFontColor method

Définit la couleur de la police sur la cellule. Pour améliorer les performances, implémentez la méthode "SetFontColor", n'implémentez pas la propriété "FontColor".

```csharp
public void SetFontColor(Color color)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| color | Color | couleur de police à définir. |

### Exemples

```csharp
[C#]
GridCell cell = gridDesktop1.GetActiveWorksheet().Cells[0, 0];
Font font = new Font("Courier New", 8, FontStyle.Italic);
cell.SetFont(font);
Color color = cell.GetFontColor();
color = Color.Black;
cell.SetFontColor(color);

[Visual Basic]
Dim cell As GridCell =  gridDesktop1.GetActiveWorksheet().Cells(0, 0) 
Dim font As Font =  New Font("Courier New",8,FontStyle.Italic) 
cell.SetFont(font)
Dim color As Color =  cell.GetFontColor() 
color = Color.Black
cell.SetFontColor(color)

```

### Voir également

* class [GridCell](../../gridcell)
* espace de noms [Aspose.Cells.GridDesktop.Data](../../gridcell)
* Assemblée [Aspose.Cells.GridDesktop](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.GridDesktop.dll -->
