---
title: "GridCell.Formula"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "GridCell propriété. Obtient ou définit une formule de la Cell"
type: docs
url: /fr/net/aspose.cells.griddesktop.data/gridcell/formula/
---
## GridCell.Formula property

Obtient ou définit une formule de la cellule.

```csharp
public string Formula { get; set; }
```

### Remarques

Une chaîne de formule commence toujours par un signe égal (=). Et veuillez toujours utiliser la virgule (,) comme délimiteur de paramètres, par exemple "=SUM(A1, E1, H2)".

L'utilisateur peut définir n'importe quelle formule dans le fichier de conception Workbook. Aspose.Cells conservera toutes les formules. Si l'utilisateur utilise cette propriété pour définir une formule dans une cellule, la majeure partie des fonctions intégrées de Workbook est prise en charge. Et davantage arrive. Si vous avez des besoins spécifiques concernant les fonctions intégrées de Workbook, veuillez nous le faire savoir.

### Exemples

```csharp
[C#]
	cell.Formula = "=SUM(A1:C3) + E6*2";
[Visual Basic]
	cell.Formula = "=SUM(A1:C3) + E6*2"
```

### Voir aussi

* class [GridCell](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)


