---
title: CellEventStringHandler
second_title: Référence de l'API Aspose.Cells pour .NET
description: Représente la méthode qui a lintention de gérer les événements de cellule. identique à linterface CellEventHandler mais renvoie la chaîne result
type: docs
weight: 340
url: /fr/net/aspose.cells.griddesktop.data/celleventstringhandler/
---
## CellEventStringHandler delegate

Représente la méthode qui a l'intention de gérer les événements de cellule. identique à l'interface CellEventHandler, mais renvoie la chaîne result

Chaîne de caractères **handleCellEvent**(Expéditeur d'objet, CellEventArgs e);

```csharp
public delegate string CellEventStringHandler(object sender, CellEventArgs e);
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| sender | Object | La grille source de l'événement. |
| e | CellEventArgs | L'argument de l'événement. L'e.Cell est la cellule qui déclenche l'événement. Le e.Argument contient l'argument de l'événement. |

### Return_Value

valeur de chaîne

### Voir également

* class [CellEventArgs](../../aspose.cells.griddesktop/celleventargs)
* espace de noms [Aspose.Cells.GridDesktop.Data](../../aspose.cells.griddesktop.data)
* Assemblée [Aspose.Cells.GridDesktop](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.GridDesktop.dll -->