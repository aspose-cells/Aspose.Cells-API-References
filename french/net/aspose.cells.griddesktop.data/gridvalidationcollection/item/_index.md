---
title: "GridValidationCollection.Item"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété GridValidationCollection. Obtient l'élément Hyperlink à l'index spécifié."
type: docs
url: /fr/net/aspose.cells.griddesktop.data/gridvalidationcollection/item/
---
## GridValidationCollection indexer (1 of 2)

Obtient l'élément Hyperlink à l'index spécifié.

```csharp
public GridValidation this[int index] { get; }
```

| Paramètre | Description |
| --- | --- |
| indice | L'indice à base zéro de l'élément. |

### Valeur de retour

L’élément à l’index spécifié.

### Voir aussi

* class [GridValidation](../../gridvalidation/)
* class [GridValidationCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## GridValidationCollection indexer (2 of 2)

Obtient l'élément [`GridValidation`](../../gridvalidation/) à la cellule spécifiée. Si aucune validation, renvoie null.

```csharp
public GridValidation this[int row, int column] { get; }
```

| Paramètre | Description |
| --- | --- |
| ligne | La ligne de la cellule. |
| column | La colonne de la cellule. |

### Valeur de retour

L’élément à l’index spécifié.

### Remarques

S'il n'existe pas d'objet de validation à l'index de ligne et de colonne spécifié, cela vérifiera l'objet de validation de la colonne.

### Voir aussi

* class [GridValidation](../../gridvalidation/)
* class [GridValidationCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)


