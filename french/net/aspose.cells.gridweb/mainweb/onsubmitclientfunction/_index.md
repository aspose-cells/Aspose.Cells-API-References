---
title: "MainWeb.OnSubmitClientFunction"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "MainWeb propriété. Obtient ou définit la fonction client à appeler avant que le contrôle ne soit soumis côté client. La fonction client doit être déclarée ainsi function MyOnSubmitarg cancelEdit  return true L'arg est l'argument de soumission contenant la commande à envoyer au serveur. Le cancelEdit est une valeur booléenne indiquant si le contrôle a ignoré l'entrée utilisateur avant la soumission. Le contrôle continuera de soumettre si la fonction renvoie true. Note Vous pouvez utiliser le pointeur this dans la fonction client pour référencer le contrôle de grille qui déclenche l'événement"
type: docs
url: /fr/net/aspose.cells.gridweb/mainweb/onsubmitclientfunction/
---
## MainWeb.OnSubmitClientFunction property

Obtient ou définit la fonction client à appeler avant que le contrôle ne soit soumis côté client. La fonction client doit être déclarée ainsi : function MyOnSubmit(arg, cancelEdit) { return true;} L'argument arg est l'argument de soumission, contenant la commande à envoyer au serveur. Le booléen cancelEdit indique si le contrôle a abandonné l'entrée utilisateur avant la soumission. Le contrôle continuera à soumettre si la fonction renvoie true. Note : Vous pouvez utiliser le pointeur \"this\" dans la fonction client pour référencer le contrôle de grille qui déclenche l'événement.

```csharp
public string OnSubmitClientFunction { get; set; }
```

### Voir aussi

* class [MainWeb](../)
* namespace [Aspose.Cells.GridWeb](../../../aspose.cells.gridweb/)
* assembly [Aspose.Cells.GridWeb](../../../)


