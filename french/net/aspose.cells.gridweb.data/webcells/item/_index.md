---
title: "WebCells.Item"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "WebCells propriété. Obtient l'élément Cell à l'index de ligne et de colonne de cellule spécifiés"
type: docs
url: /fr/net/aspose.cells.gridweb.data/webcells/item/
---
## WebCells indexer (1 of 2)

Obtient l'élément Cell à l'index de ligne et de colonne de cellule spécifiés.

```csharp
public WebCell this[int row, int column] { get; }
```

| Paramètre | Description |
| --- | --- |
| ligne | Index de ligne. |
| column | Index de colonne. |

### Valeur de retour

L'objet Cell.

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

* class [WebCell](../../webcell/)
* class [WebCells](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)

---

## WebCells indexer (2 of 2)

Obtient l'élément Cell au nom de cellule spécifié.

```csharp
public WebCell this[string cellName] { get; }
```

| Paramètre | Description |
| --- | --- |
| cellName | Nom de cellule, incluant sa lettre de colonne et son numéro de ligne, par exemple A5. |

### Valeur de retour

Un objet Cell

### Exemples

```csharp
[C#]

Cells cells = excel.Worksheets[0].Cells;
Cell cell = cells["A1"];	//Gets the cell at "A1"

[Visual Basic]

Dim cells As Cells =  excel.Worksheets(0).Cells
Dim cell As Cell =  cells("A1")  'Gets the cell at "A1"
```

### Voir aussi

* class [WebCell](../../webcell/)
* class [WebCells](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)


