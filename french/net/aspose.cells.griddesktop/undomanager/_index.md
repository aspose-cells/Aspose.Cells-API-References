---
title: "Classe UndoManager"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.GridDesktop.UndoManager class. Encapsule l'objet qui gère les opérations d'annulation/rétablissement"
type: docs
url: /fr/net/aspose.cells.griddesktop/undomanager/
---
## UndoManager class

Encapsule l'objet qui gère les opérations d'annulation/restauration.

```csharp
public class UndoManager
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Enabled](../../aspose.cells.griddesktop/undomanager/enabled/) { get; set; } | Obtient ou définit une valeur indiquant si la fonction Undo est activée. La valeur par défaut est false. |
| [RedoStepsCount](../../aspose.cells.griddesktop/undomanager/redostepscount/) { get; } | Obtient le nombre actuel d'étapes de rétablissement disponibles. |
| [UndoStackSize](../../aspose.cells.griddesktop/undomanager/undostacksize/) { get; set; } | Obtient ou définit la taille de la pile d'annulation/rétablissement. La valeur par défaut est 300. |
| [UndoStepsCount](../../aspose.cells.griddesktop/undomanager/undostepscount/) { get; } | Obtient le nombre actuel d'étapes d'annulation disponibles. |

## Méthodes

| Nom | Description |
| --- | --- |
| [BeginChanges](../../aspose.cells.griddesktop/undomanager/beginchanges/)() | Commence à enregistrer les modifications. |
| [BeginMark](../../aspose.cells.griddesktop/undomanager/beginmark/)() | Commence à marquer les modifications. |
| [ClearStack](../../aspose.cells.griddesktop/undomanager/clearstack/)() | Efface les piles d'Undo et de Redo. |
| [EndChanges](../../aspose.cells.griddesktop/undomanager/endchanges/)() | Termine l'enregistrement des modifications. |
| [EndMark](../../aspose.cells.griddesktop/undomanager/endmark/)() | Termine le marquage des modifications. |
| [Redo](../../aspose.cells.griddesktop/undomanager/redo/)() | Effectue une opération de redo. |
| [RedoMark](../../aspose.cells.griddesktop/undomanager/redomark/)() | Effectue une opération de redo avec marquage. |
| [Undo](../../aspose.cells.griddesktop/undomanager/undo/)() | Effectue une opération d'undo. |
| [UndoMark](../../aspose.cells.griddesktop/undomanager/undomark/)() | Effectue une opération d'undo avec marquage. |

### Voir aussi

* namespace [Aspose.Cells.GridDesktop](../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../)


