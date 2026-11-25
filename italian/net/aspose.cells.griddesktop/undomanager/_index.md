---
title: "Classe UndoManager"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.GridDesktop.UndoManager class. Incapsula l'oggetto che gestisce le operazioni di undo/redo"
type: docs
url: /it/net/aspose.cells.griddesktop/undomanager/
---
## UndoManager class

Incapsula l'oggetto che gestisce le operazioni di annullamento/ripristino.

```csharp
public class UndoManager
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Enabled](../../aspose.cells.griddesktop/undomanager/enabled/) { get; set; } | Ottiene o imposta un valore che indica se la funzione Undo è abilitata. Il valore predefinito è false. |
| [RedoStepsCount](../../aspose.cells.griddesktop/undomanager/redostepscount/) { get; } | Ottiene il conteggio attuale dei passaggi redo disponibili. |
| [UndoStackSize](../../aspose.cells.griddesktop/undomanager/undostacksize/) { get; set; } | Ottiene o imposta la dimensione dello stack undo/redo. Il valore predefinito è 300. |
| [UndoStepsCount](../../aspose.cells.griddesktop/undomanager/undostepscount/) { get; } | Ottiene il conteggio attuale dei passaggi undo disponibili. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [BeginChanges](../../aspose.cells.griddesktop/undomanager/beginchanges/)() | Inizia a registrare le modifiche. |
| [BeginMark](../../aspose.cells.griddesktop/undomanager/beginmark/)() | Inizia a contrassegnare le modifiche. |
| [ClearStack](../../aspose.cells.griddesktop/undomanager/clearstack/)() | Cancella gli stack Undo e Redo. |
| [EndChanges](../../aspose.cells.griddesktop/undomanager/endchanges/)() | Termina la registrazione delle modifiche. |
| [EndMark](../../aspose.cells.griddesktop/undomanager/endmark/)() | Termina il contrassegno delle modifiche. |
| [Redo](../../aspose.cells.griddesktop/undomanager/redo/)() | Esegue un'operazione redo. |
| [RedoMark](../../aspose.cells.griddesktop/undomanager/redomark/)() | Esegue un'operazione redo con contrassegno. |
| [Undo](../../aspose.cells.griddesktop/undomanager/undo/)() | Esegue un'operazione undo. |
| [UndoMark](../../aspose.cells.griddesktop/undomanager/undomark/)() | Esegue un'operazione undo con contrassegno. |

### Vedi anche

* namespace [Aspose.Cells.GridDesktop](../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../)


