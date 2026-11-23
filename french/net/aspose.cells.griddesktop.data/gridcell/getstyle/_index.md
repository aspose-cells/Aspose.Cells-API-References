---
title: "GridCell.GetStyle"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode GridCell. Obtient le style de la cellule. Lorsque vous modifiez le style, vous devez appeler la méthode SetStyle pour appliquer le style à la cellule."
type: docs
url: /fr/net/aspose.cells.griddesktop.data/gridcell/getstyle/
---
## GridCell.GetStyle method

Obtient le style de la cellule. Lors du changement du style, vous devez appeler la méthode "SetStyle" pour appliquer le style à la cellule.

```csharp
public Style GetStyle()
```

### Valeur de retour

renvoie une copie du style de la cellule.

### Exemples

```csharp
[C#]
Style style = sheet.GetCell(0, 0).GetStyle();
style.CellLocked = true;
style.VAlignment = VerticalAlignmentType.Top;
...
sheet.GetCell(0, 0).SetStyle(style);

[Visual Basic]
Dim style As Style =  sheet.GetCell(0,0).GetStyle() 
style.CellLocked = True
style.VAlignment = VerticalAlignmentType.Top
...
sheet.GetCell(0, 0).SetStyle(style)

```

### Voir aussi

* class [Style](../../../aspose.cells.griddesktop/style/)
* class [GridCell](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)


