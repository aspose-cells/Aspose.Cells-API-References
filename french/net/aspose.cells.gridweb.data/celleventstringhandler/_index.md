---
title: "Délégué CellEventStringHandler"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Représente la méthode qui a pour but de gérer les événements de cellule. même que l'interface CellEventHandler mais renvoie un résultat de type chaîne"
type: docs
url: /fr/net/aspose.cells.gridweb.data/celleventstringhandler/
---
## CellEventStringHandler delegate

Représente la méthode destinée à gérer les événements de cellule. identique à l'interface CellEventHandler, mais renvoie un résultat de type chaîne.

String **handleCellEvent**(Object sender, CellEventArgs e);

```csharp
public delegate string CellEventStringHandler(object sender, CellEventArgs e);
```

| Paramètre | Type | Description |
| --- | --- | --- |
| sender | Object | La grille source de l'événement. |
| e | CellEventArgs | L'argument de l'événement. e.Cell est la cellule qui déclenche l'événement. e.Argument contient l'argument de l'événement. |

### Valeur de retour

string value

### Voir aussi

* class [CellEventArgs](../../aspose.cells.gridweb/celleventargs/)
* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


