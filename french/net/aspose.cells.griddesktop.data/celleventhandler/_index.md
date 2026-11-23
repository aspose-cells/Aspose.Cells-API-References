---
title: "Délégué CellEventHandler"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Représente l'interface qui a pour but de gérer les événements de cellule"
type: docs
url: /fr/net/aspose.cells.griddesktop.data/celleventhandler/
---
## CellEventHandler delegate

Représente l'interface destinée à gérer les événements de cellule.

void **handleCellEvent**(Object sender, CellEventArgs e);

```csharp
public delegate void CellEventHandler(object sender, CellEventArgs e);
```

| Paramètre | Type | Description |
| --- | --- | --- |
| sender | Object | La grille source de l'événement. |
| e | CellEventArgs | L'argument de l'événement. e.Cell est la cellule qui déclenche l'événement. e.Argument contient l'argument de l'événement. |

### Voir aussi

* class [CellEventArgs](../../aspose.cells.griddesktop/celleventargs/)
* namespace [Aspose.Cells.GridDesktop.Data](../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../)


