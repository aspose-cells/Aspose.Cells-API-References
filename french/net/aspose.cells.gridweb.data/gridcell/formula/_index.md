---
title: "GridCell.Formula"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété GridCell. Obtient ou définit une formule du GridCell"
type: docs
url: /fr/net/aspose.cells.gridweb.data/gridcell/formula/
---
## GridCell.Formula property

Obtient ou définit une formule du [`GridCell`](../).

```csharp
public string Formula { get; set; }
```

### Remarques

Une chaîne de formule commence toujours par un signe égal (=). Et veuillez toujours utiliser la virgule (,) comme délimiteur de paramètres, par exemple "=SUM(A1, E1, H2)".

L'utilisateur peut définir n'importe quelle formule dans le fichier de conception Workbook. Aspose.Cells conservera toutes les formules. Si l'utilisateur utilise cette propriété pour définir une formule dans une cellule, la majeure partie des fonctions intégrées de Workbook est prise en charge. Et davantage arrive. Si vous avez des besoins spécifiques concernant les fonctions intégrées de Workbook, veuillez nous le faire savoir.

### Exemples

```csharp
[C#]

ridWeb GridWeb1 = new GridWeb();
ridWorksheet sheet = GridWeb1.ActiveSheet;
heet.Cells["B6"].Formula = "=SUM(B2:B5, E1) + sheet1!A1";

Visual Basic]

im GridWeb1 As GridWeb =  New GridWeb() 
im sheet As GridWorksheet =  GridWeb1.ActiveSheet 
heet.Cells["B6"].Formula = "=SUM(B2:B5, E1) + sheet1!A1"
```

### Voir aussi

* class [GridCell](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)


