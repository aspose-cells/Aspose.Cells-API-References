---
title: "Clase RevisionCellComment"
linktitle: "RevisionCellComment"
second_title: "Aspose.Cells for Go via C++ API Reference"
description: "Clase RevisionCellComment. Encapsula el objeto que representa un comentario de revisión en Go."
type: docs
weight: 200
url: /es/go-cpp/revisioncellcomment/
---

## RevisionCellComment class

Represents a revision record of a cell comment change.

```go

type RevisionCellComment struct  {
	ptr unsafe.Pointer
}

```
## Constructors

| Method | Description |
| --- | --- |
| [NewRevisionCellComment](./newrevisioncellcomment/) | Constructs from a parent object. |

## Methods

| Method | Description |
| --- | --- |
| [IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
| [GetType](./gettype/) | Gets the type of revision. |
| [GetRow](./getrow/) | Obtiene el índice de fila que contiene un comentario. |
| [GetColumn](./getcolumn/) | Obtiene el índice de columna que contiene un comentario. |
| [GetCellName](./getcellname/) | Gets the name of the cell. |
| [SetCellName](./setcellname/) | Gets the name of the cell. |
| [GetActionType](./getactiontype/) | Obtiene el tipo de acción de la revisión. |
| [IsOldComment](./isoldcomment/) | Indica si es un comentario antiguo. |
| [GetOldLength](./getoldlength/) | Obtiene la longitud del texto del comentario añadido en esta revisión. |
| [GetNewLength](./getnewlength/) | Obtiene la longitud del comentario antes de que se hiciera esta revisión. |
| [GetWorksheet](./getworksheet/) | Gets the worksheet. |
| [GetId](./getid/) | Gets the number of this revision. |
