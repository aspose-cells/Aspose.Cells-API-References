---
title: "CellControlCollection.Item"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété CellControlCollection. Obtient le contrôle de cellule à l'index de ligne et de colonne spécifié."
type: docs
url: /fr/net/aspose.cells.griddesktop/cellcontrolcollection/item/
---
## CellControlCollection indexer (1 of 2)

Obtient le contrôle de cellule à l'index de ligne et de colonne spécifié.

```csharp
public CellControl this[int row, int col] { get; }
```

| Paramètre | Description |
| --- | --- |
| ligne | index de ligne. |
| col | index de colonne. |

### Remarques

S'il n'existe pas d'objet CellControl à l'index de ligne et de colonne spécifié, cela vérifiera l'objet CellControl de la colonne.

### Voir aussi

* class [CellControl](../../cellcontrol/)
* class [CellControlCollection](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## CellControlCollection indexer (2 of 2)

Obtient le contrôle de cellule par le nom de cellule spécifié.

```csharp
public CellControl this[string cellName] { get; }
```

| Paramètre | Description |
| --- | --- |
| cellName | nom de cellule (au format de nom Excel, comme 'A1', 'F22') |

### Remarques

S'il n'existe pas d'objet CellControl à l'index de ligne et de colonne spécifié, cela vérifiera l'objet CellControl de la colonne.

### Voir aussi

* class [CellControl](../../cellcontrol/)
* class [CellControlCollection](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)


