---
title: "Delegate RowColumnEventHandler"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Représente l'interface qui a pour but de gérer les événements de ligne/colonne"
type: docs
url: /fr/net/aspose.cells.griddesktop.data/rowcolumneventhandler/
---
## RowColumnEventHandler delegate

Représente l'interface destinée à gérer les événements de ligne/colonne.

void **handleCellEvent**(Object sender, RowColumnEventArgs e);

```csharp
public delegate void RowColumnEventHandler(object sender, RowColumnEventArgs e);
```

| Paramètre | Type | Description |
| --- | --- | --- |
| sender | Object | La source de l'événement. |
| e | RowColumnEventArgs | L'argument de l'événement. Appelez e.RejectOperation() si vous souhaitez annuler l'opération de suppression dans les gestionnaires d'événements RowDeleting ou ColumnDeleting. |

### Voir aussi

* class [RowColumnEventArgs](../../aspose.cells.griddesktop/rowcolumneventargs/)
* namespace [Aspose.Cells.GridDesktop.Data](../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../)


