---
title: "GridCell.GetFontColor"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "GridCell méthode. Obtient la couleur de police de la cellule. Lorsqu'on change la couleur, vous devez appeler la méthode SetFontColor pour définir la couleur de police de la cellule."
type: docs
url: /fr/net/aspose.cells.griddesktop.data/gridcell/getfontcolor/
---
## GridCell.GetFontColor method

Obtient la couleur de police de la cellule. Lors du changement de la couleur, vous devez appeler la méthode "SetFontColor" pour appliquer la couleur de police à la cellule.

```csharp
public Color GetFontColor()
```

### Valeur de retour

renvoie la couleur de police de la cellule.

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


