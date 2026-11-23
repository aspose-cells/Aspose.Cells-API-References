---
title: "Délégué CellErrorHandler"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Représente l'interface qui a pour but de gérer les événements d'erreur de cellule"
type: docs
url: /fr/net/aspose.cells.gridweb.data/cellerrorhandler/
---
## CellErrorHandler delegate

Représente l'interface destinée à gérer les événements d'erreur de cellule.

void **handleCellEvent**(Object sender, GridCellException ex, OnErrorActionQuery query);

```csharp
public delegate void CellErrorHandler(object sender, WebCellException ex, 
    OnErrorActionQuery action);
```

| Paramètre | Type | Description |
| --- | --- | --- |
| sender | Object | La source de l'événement. |
| ex | WebCellException | L'erreur d'opération de cellule. |
| action | OnErrorActionQuery | peut obtenir des informations sur le type d'action onerror. |

### Voir aussi

* class [WebCellException](../webcellexception/)
* class [OnErrorActionQuery](../onerroractionquery/)
* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


