---
title: "GridCell.SetStyle"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "GridCell méthode. Définit le style de la cellule. Pour améliorer les performances, implémentez la méthode SetStyle plutôt que d'implémenter la propriété Style"
type: docs
url: /fr/net/aspose.cells.griddesktop.data/gridcell/setstyle/
---
## GridCell.SetStyle method

Définit le style de la cellule. Pour améliorer les performances, implémentez la méthode "SetStyle", n'implémentez pas la propriété "Style".

```csharp
public void SetStyle(Style value)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| style | Style | style à définir. |

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


