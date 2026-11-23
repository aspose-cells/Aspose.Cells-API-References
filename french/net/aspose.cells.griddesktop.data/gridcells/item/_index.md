---
title: "GridCells.Item"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété GridCells. Obtient l'élément GridCell à l'index de ligne et de colonne de cellule spécifié"
type: docs
url: /fr/net/aspose.cells.griddesktop.data/gridcells/item/
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

Cells cells = excel.Worksheets[0].Cells;
Cell cell = cells[0, 0];	//Gets the cell at "A1"

[Visual Basic]

Dim cells As Cells =  excel.WorkSheets(0).Cells
Dim cell As Cell =  cells(0,0)  'Gets the cell at "A1"
```

### Voir aussi

* class [GridCell](../../gridcell/)
* class [GridCells](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

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

### Voir aussi

* class [GridCell](../../gridcell/)
* class [GridCells](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)


