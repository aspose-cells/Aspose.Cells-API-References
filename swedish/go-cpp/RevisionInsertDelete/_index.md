---
title: "RevisionInsertDelete klass"
linktitle: "RevisionInsertDelete"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "RevisionInsertDelete klass. Inkapslar objektet som representerar revisioninsertdelete i Go."
type: docs
weight: 200
url: /sv/go-cpp/revisioninsertdelete/
---

## RevisionInsertDelete class

Representerar en revisionspost för en rad/kolumn infogning/borttagningsåtgärd.

```go

type RevisionInsertDelete struct  {
	ptr unsafe.Pointer
}

```
## Konstruktörer

| Metod | Beskrivning |
| --- | --- |
| [NewRevisionInsertDelete](./newrevisioninsertdelete/) | Skapas från ett föräldraobjekt. |

## Metoder

| Metod | Beskrivning |
| --- | --- |
| [IsNull](./isnull/) | Kontrollerar om implementeringsobjektet är nullptr. |
| [GetType](./gettype/) | Representerar revisionstypen. |
| [GetCellArea](./getcellarea/) | Hämtar det insättnings-/raderingsintervallet. |
| [GetActionType](./getactiontype/) | Hämtar åtgärdstypen för denna revision. |
| [GetRevisions](./getrevisions/) | Hämtar revisionslistan för denna operation. |
| [GetWorksheet](./getworksheet/) | Hämtar arbetsbladet. |
| [GetId](./getid/) | Hämtar numret för denna revision. |
