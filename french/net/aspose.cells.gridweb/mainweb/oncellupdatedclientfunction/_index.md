---
title: "MainWeb.OnCellUpdatedClientFunction"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "MainWeb propriété. Obtient ou définit le nom de la fonction côté client à appeler lorsqu'une valeur de cellule est mise à jour. La fonction client doit être déclarée ainsi : function MyOnCellUpdatedcell  alertthis.getCellValueByCellcell Note Vous pouvez utiliser le pointeur this dans la fonction client pour pointer le contrôle de grille qui déclenche l'événement"
type: docs
url: /fr/net/aspose.cells.gridweb/mainweb/oncellupdatedclientfunction/
---
## MainWeb.OnCellUpdatedClientFunction property

Obtient ou définit le nom de la fonction côté client à appeler lorsqu'une valeur de cellule est mise à jour. La fonction client doit être déclarée ainsi : function MyOnCellUpdated(cell) { alert(this.getCellValueByCell(cell)); } Note : Vous pouvez utiliser le pointeur "this" dans la fonction client pour référencer le contrôle de grille qui déclenche l'événement.

```csharp
public string OnCellUpdatedClientFunction { get; set; }
```

### Voir aussi

* class [MainWeb](../)
* namespace [Aspose.Cells.GridWeb](../../../aspose.cells.gridweb/)
* assembly [Aspose.Cells.GridWeb](../../../)


