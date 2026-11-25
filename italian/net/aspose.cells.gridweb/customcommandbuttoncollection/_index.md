---
title: "Classe CustomCommandButtonCollection"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.GridWeb.CustomCommandButtonCollection. Rappresenta la raccolta di CustomCommandButton"
type: docs
url: /it/net/aspose.cells.gridweb/customcommandbuttoncollection/
---
## CustomCommandButtonCollection class

Rappresenta la raccolta di CustomCommandButton.

```csharp
public class CustomCommandButtonCollection : CollectionBase
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Count](../../aspose.cells.gridweb/customcommandbuttoncollection/count/) { get; } | Ottiene il conteggio della raccolta. |
| [IsFixedSize](../../aspose.cells.gridweb/customcommandbuttoncollection/isfixedsize/) { get; } | Utilizzato solo internamente. |
| [IsReadOnly](../../aspose.cells.gridweb/customcommandbuttoncollection/isreadonly/) { get; } | Utilizzato solo internamente. |
| [IsSynchronized](../../aspose.cells.gridweb/customcommandbuttoncollection/issynchronized/) { get; } | Utilizzato solo internamente. |
| [Item](../../aspose.cells.gridweb/customcommandbuttoncollection/item/) { get; set; } | Ottiene un oggetto custom command button all'indice. |
| [SyncRoot](../../aspose.cells.gridweb/customcommandbuttoncollection/syncroot/) { get; } | Utilizzato solo internamente. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Add](../../aspose.cells.gridweb/customcommandbuttoncollection/add/)(object) | Aggiunge un oggetto custom command button alla raccolta. |
| [Clear](../../aspose.cells.gridweb/customcommandbuttoncollection/clear/#clear)() | Cancella la raccolta. |
| [Contains](../../aspose.cells.gridweb/customcommandbuttoncollection/contains/)(object) | Indica se l'oggetto pulsante di comando personalizzato è nella collezione. |
| [CopyTo](../../aspose.cells.gridweb/customcommandbuttoncollection/copyto/)(Array, int) | Copia la collezione in un array. |
| [GetEnumerator](../../aspose.cells.gridweb/customcommandbuttoncollection/getenumerator/#getenumerator)() | Ottiene un oggetto IEnumerator della collezione. |
| [IndexOf](../../aspose.cells.gridweb/customcommandbuttoncollection/indexof/)(object) | Ottiene l'indice del pulsante. |
| [Insert](../../aspose.cells.gridweb/customcommandbuttoncollection/insert/)(int, object) | Inserisce un pulsante all'indice. |
| [Remove](../../aspose.cells.gridweb/customcommandbuttoncollection/remove/)(object) | Rimuove l'oggetto pulsante di comando personalizzato. |
| [RemoveAt](../../aspose.cells.gridweb/customcommandbuttoncollection/removeat/#removeat)(int) | Rimuove all'indice. |

### Esempi

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

### Vedi anche

* namespace [Aspose.Cells.GridWeb](../../aspose.cells.gridweb/)
* assembly [Aspose.Cells.GridWeb](../../)


