---
title: "GridCell.GetFont"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode GridCell. Obtient la police de la cellule. Lorsque vous modifiez la police, vous devez appeler la méthode SetFont pour appliquer la police à la cellule."
type: docs
url: /fr/net/aspose.cells.griddesktop.data/gridcell/getfont/
---
## GridCell.GetFont method

Obtient la police de la cellule. Lors du changement de la police, vous devez appeler la méthode "SetFont" pour appliquer la police à la cellule.

```csharp
public Font GetFont()
```

### Valeur de retour

renvoie une copie de la police de la cellule.

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


