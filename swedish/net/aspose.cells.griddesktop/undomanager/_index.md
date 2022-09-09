---
title: UndoManager
second_title: Aspose.Cells för .NET API-referens
description: Kapslar in objektet som hanterar ångra/gör om-operationerna.
type: docs
weight: 1030
url: /sv/net/aspose.cells.griddesktop/undomanager/
---
## UndoManager class

Kapslar in objektet som hanterar ångra/gör om-operationerna.

```csharp
public class UndoManager
```

## Egenskaper

| namn | Beskrivning |
| --- | --- |
| [Enabled](../../aspose.cells.griddesktop/undomanager/enabled) { get; set; } | Hämtar eller ställer in ett värde som indikerar om funktionen Ångra är aktiverad. Standardvärdet är false. |
| [RedoStepsCount](../../aspose.cells.griddesktop/undomanager/redostepscount) { get; } | Hämtar det aktuella antalet redogöringssteg. |
| [UndoStackSize](../../aspose.cells.griddesktop/undomanager/undostacksize) { get; set; } | Hämtar eller ställer in stackstorleken för ångra/gör om. Standardvärdet är 300. |
| [UndoStepsCount](../../aspose.cells.griddesktop/undomanager/undostepscount) { get; } | Får aktuellt antal tillgängliga ångra steg. |

## Metoder

| namn | Beskrivning |
| --- | --- |
| [BeginChanges](../../aspose.cells.griddesktop/undomanager/beginchanges)() | Börjar registrera ändringar. |
| [BeginMark](../../aspose.cells.griddesktop/undomanager/beginmark)() | Börjar markera ändringar. |
| [ClearStack](../../aspose.cells.griddesktop/undomanager/clearstack)() | Rensar stackarna Ångra och Gör om. |
| [EndChanges](../../aspose.cells.griddesktop/undomanager/endchanges)() | Slutar för att registrera ändringar. |
| [EndMark](../../aspose.cells.griddesktop/undomanager/endmark)() | Slutar för att markera ändringar. |
| [Redo](../../aspose.cells.griddesktop/undomanager/redo)() | Utför en redo-operation. |
| [RedoMark](../../aspose.cells.griddesktop/undomanager/redomark)() | Utför en redo-operation med mark. |
| [Undo](../../aspose.cells.griddesktop/undomanager/undo)() | Utför en ångra-åtgärd. |
| [UndoMark](../../aspose.cells.griddesktop/undomanager/undomark)() | Utför en ångra-operation med mark. |

### Se även

* namnutrymme [Aspose.Cells.GridDesktop](../../aspose.cells.griddesktop)
* hopsättning [Aspose.Cells.GridDesktop](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.GridDesktop.dll -->