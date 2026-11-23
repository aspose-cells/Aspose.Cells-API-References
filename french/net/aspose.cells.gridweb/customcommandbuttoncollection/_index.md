---
title: "Classe CustomCommandButtonCollection"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.GridWeb.CustomCommandButtonCollection. Représente la collection de CustomCommandButton"
type: docs
url: /fr/net/aspose.cells.gridweb/customcommandbuttoncollection/
---
## CustomCommandButtonCollection class

Représente la collection de CustomCommandButton.

```csharp
public class CustomCommandButtonCollection : CollectionBase
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Count](../../aspose.cells.gridweb/customcommandbuttoncollection/count/) { get; } | Obtient le nombre d'éléments de la collection. |
| [IsFixedSize](../../aspose.cells.gridweb/customcommandbuttoncollection/isfixedsize/) { get; } | Utilisé uniquement en interne. |
| [IsReadOnly](../../aspose.cells.gridweb/customcommandbuttoncollection/isreadonly/) { get; } | Utilisé uniquement en interne. |
| [IsSynchronized](../../aspose.cells.gridweb/customcommandbuttoncollection/issynchronized/) { get; } | Utilisé uniquement en interne. |
| [Item](../../aspose.cells.gridweb/customcommandbuttoncollection/item/) { get; set; } | Obtient un objet de bouton de commande personnalisé à l'index. |
| [SyncRoot](../../aspose.cells.gridweb/customcommandbuttoncollection/syncroot/) { get; } | Utilisé uniquement en interne. |

## Méthodes

| Nom | Description |
| --- | --- |
| [Add](../../aspose.cells.gridweb/customcommandbuttoncollection/add/)(object) | Ajoute un objet de bouton de commande personnalisé à la collection. |
| [Clear](../../aspose.cells.gridweb/customcommandbuttoncollection/clear/#clear)() | Efface la collection. |
| [Contains](../../aspose.cells.gridweb/customcommandbuttoncollection/contains/)(object) | Indique si l'objet bouton de commande personnalisé se trouve dans la collection. |
| [CopyTo](../../aspose.cells.gridweb/customcommandbuttoncollection/copyto/)(Array, int) | Copie la collection dans un tableau. |
| [GetEnumerator](../../aspose.cells.gridweb/customcommandbuttoncollection/getenumerator/#getenumerator)() | Obtient un objet IEnumerator de la collection. |
| [IndexOf](../../aspose.cells.gridweb/customcommandbuttoncollection/indexof/)(object) | Obtient l'index du bouton. |
| [Insert](../../aspose.cells.gridweb/customcommandbuttoncollection/insert/)(int, object) | Insère un bouton à l'index. |
| [Remove](../../aspose.cells.gridweb/customcommandbuttoncollection/remove/)(object) | Supprime l'objet bouton de commande personnalisé. |
| [RemoveAt](../../aspose.cells.gridweb/customcommandbuttoncollection/removeat/#removeat)(int) | Supprime à l'index. |

### Exemples

```csharp
[C#]
GridWeb GridWeb1 = new GridWeb();
CustomCommandButton button = new CustomCommandButton();
button.Command = "MyCommand";
button.ImageUrl = "images/button1.gif";
GridWeb1.CustomCommandButtons.Add(button);
[VB]
Dim GridWeb1 As GridWeb= New GridWeb();
Dim button As CustomCommandButton =  New CustomCommandButton()
button.Command = "MyCommand"
button.ImageUrl = "images/button1.gif"
GridWeb1.CustomCommandButtons.Add(button)
```

### Voir aussi

* namespace [Aspose.Cells.GridWeb](../../aspose.cells.gridweb/)
* assembly [Aspose.Cells.GridWeb](../../)


