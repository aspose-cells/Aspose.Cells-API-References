---
title: RevisionInsertDelete Class 
linktitle: RevisionInsertDelete
second_title: Aspose.Cells for Go via C++ API Reference
description: 'RevisionInsertDelete class. Encapsulates the object that represents revisioninsertdelete in Go.'
type: docs
weight: 200
url: /go-cpp/revisioninsertdelete/
---

## RevisionInsertDelete class

Represents a revision record of a row/column insert/delete action.

```go

type RevisionInsertDelete struct  {
	ptr unsafe.Pointer
}

```
## Constructors

| Method | Description |
| --- | --- |
|[NewRevisionInsertDelete](./newrevisioninsertdelete/) | Constructs from a parent object. | 

## Methods

| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. | 
|[GetType](./gettype/) | Represents the type of revision. | 
|[GetCellArea](./getcellarea/) | Gets the inserting/deleting range. | 
|[GetActionType](./getactiontype/) | Gets the action type of this revision. | 
|[GetRevisions](./getrevisions/) | Gets revision list by this operation. | 
|[GetWorksheet](./getworksheet/) | Gets the worksheet. | 
|[GetId](./getid/) | Gets the number of this revision. | 
