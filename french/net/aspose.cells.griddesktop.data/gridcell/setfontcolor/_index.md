---
title: "GridCell.SetFontColor"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode GridCell. Définit la couleur de la police de la cellule. Pour améliorer les performances, implémentez la méthode SetFontColor au lieu d'implémenter la propriété FontColor."
type: docs
url: /fr/net/aspose.cells.griddesktop.data/gridcell/setfontcolor/
---
## GridCell.SetFontColor method

Définit la couleur de police de la cellule. Pour améliorer les performances, implémentez la méthode "SetFontColor", n'implémentez pas la propriété "FontColor".

```csharp
public void SetFontColor(Color color)
```

| Paramètre | Type | Description |
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

### Voir aussi

* class [GridCell](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)


