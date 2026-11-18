---
title: "RevisionCellComment klass"
linktitle: "RevisionCellComment"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "RevisionCellComment klass. Innesluter objektet som representerar revisioncellcomment i Go."
type: docs
weight: 200
url: /sv/go-cpp/revisioncellcomment/
---

## RevisionCellComment class

Representerar en revisionspost för en cellkommentarsändring.

```go

type RevisionCellComment struct  {
	ptr unsafe.Pointer
}

```
## Konstruktörer

| Metod | Beskrivning |
| --- | --- |
| [NewRevisionCellComment](./newrevisioncellcomment/) | Skapas från ett föräldraobjekt. |

## Metoder

| Metod | Beskrivning |
| --- | --- |
| [IsNull](./isnull/) | Kontrollerar om implementeringsobjektet är nullptr. |
| [GetType](./gettype/) | Hämtar revisionens typ. |
| [GetRow](./getrow/) | Hämtar radindex för den som innehåller en kommentar. |
| [GetColumn](./getcolumn/) | Hämtar kolumnindex för den som innehåller en kommentar. |
| [GetCellName](./getcellname/) | Hämtar cellens namn. |
| [SetCellName](./setcellname/) | Hämtar cellens namn. |
| [GetActionType](./getactiontype/) | Hämtar åtgärdstypen för revisionen. |
| [IsOldComment](./isoldcomment/) | Indikerar om det är en gammal kommentar. |
| [GetOldLength](./getoldlength/) | Hämtar längden på kommentartexten som lagts till i denna revision. |
| [GetNewLength](./getnewlength/) | Hämtar längden på kommentaren innan denna revision gjordes. |
| [GetWorksheet](./getworksheet/) | Hämtar arbetsbladet. |
| [GetId](./getid/) | Hämtar numret för denna revision. |
