---
title: "GridCells.Item"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété GridCells. Obtient l'élément GridCell à l'index de ligne et de colonne de cellule spécifié"
type: docs
url: /fr/net/aspose.cells.gridweb.data/gridcells/item/
---
## GridCells indexer (1 of 2)

Obtient l'élément [`GridCell`](../../gridcell/) à l'index de ligne et de colonne de cellule spécifié.

```csharp
public GridCell this[int row, int column] { get; }
```

| Paramètre | Description |
| --- | --- |
| ligne | Index de ligne. |
| column | Index de colonne. |

### Valeur de retour

L'objet [`GridCell`](../../gridcell/).

### Exemples

```csharp
[C#]
GridWeb GridWeb1 = new GridWeb();
GridCells cells = GridWeb1.WorkSheets[0].Cells;
//Obtient la cellule à "A1"
GridCell cell = cells[0, 0];	

[Visual Basic]

Dim cells As Cells =  excel.WorkSheets(0).Cells
 'Gets the cell at "A1"
Dim cell As Cell =  cells(0,0) 
```

### Voir aussi

* class [GridCell](../../gridcell/)
* class [GridCells](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)

---

## GridCells indexer (2 of 2)

Obtient l'élément [`GridCell`](../../gridcell/) au nom de cellule spécifié.

```csharp
public GridCell this[string cellName] { get; }
```

| Paramètre | Description |
| --- | --- |
| cellName | Nom de cellule, incluant sa lettre de colonne et son numéro de ligne, par exemple A5. |

### Valeur de retour

Un objet [`GridCell`](../../gridcell/)

### Exemples

```csharp
[C#]
ridWeb GridWeb1 = new GridWeb();
 GridCells cells = GridWeb1.WorkSheets[0].Cells;
 GridCell cell = cells["A1"];	//Gets the cell at "A1"

[Visual Basic]

Dim cells As Cells =  excel.Worksheets(0).Cells
Dim cell As Cell =  cells("A1")  'Gets the cell at "A1"
```

### Voir aussi

* class [GridCell](../../gridcell/)
* class [GridCells](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)


