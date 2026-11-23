---
title: "MainWeb.OnContextMenuShowClientFunction"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "MainWeb propriété. Obtient ou définit la fonction côté client à appeler lorsque le menu contextuel sera affiché. La fonction client doit être déclarée ainsi function onContextMenuShow  var menu  event.srcElement menu.setItemVisibilityDelete block menu.setItemVisibilityUpdate none Note Vous pouvez utiliser le pointeur this dans la fonction client pour référencer le contrôle de grille qui déclenche l'événement"
type: docs
url: /fr/net/aspose.cells.gridweb/mainweb/oncontextmenushowclientfunction/
---
## MainWeb.OnContextMenuShowClientFunction property

Obtient ou définit la fonction côté client à appeler lorsque le menu contextuel sera affiché. La fonction client doit être déclarée ainsi : function onContextMenuShow() { var menu = event.srcElement; menu.setItemVisibility(\"Delete\", \"block\"); menu.setItemVisibility(\"Update\", \"none\"); }Note : Vous pouvez utiliser le pointeur \"this\" dans la fonction client pour référencer le contrôle de grille qui déclenche l'événement.

```csharp
public string OnContextMenuShowClientFunction { get; set; }
```

### Voir aussi

* class [MainWeb](../)
* namespace [Aspose.Cells.GridWeb](../../../aspose.cells.gridweb/)
* assembly [Aspose.Cells.GridWeb](../../../)


