---
title: "Класс RevisionInsertDelete"
linktitle: "RevisionInsertDelete"
second_title: "Справочник API Aspose.Cells for Go через C++"
description: "Класс RevisionInsertDelete. Инкапсулирует объект, представляющий revisioninsertdelete в Go."
type: docs
weight: 200
url: /ru/go-cpp/revisioninsertdelete/
---

## RevisionInsertDelete class

Представляет запись ревизии действия вставки/удаления строки/столбца.

```go

type RevisionInsertDelete struct  {
	ptr unsafe.Pointer
}

```
## Конструкторы

| Метод | Описание |
| --- | --- |
| [NewRevisionInsertDelete](./newrevisioninsertdelete/) | Создаётся из родительского объекта. |

## Методы

| Метод | Описание |
| --- | --- |
| [IsNull](./isnull/) | Проверяет, является ли объект реализации nullptr. |
| [GetType](./gettype/) | Представляет тип ревизии. |
| [GetCellArea](./getcellarea/) | Получает диапазон вставки/удаления. |
| [GetActionType](./getactiontype/) | Получает тип действия этой ревизии. |
| [GetRevisions](./getrevisions/) | Получает список ревизий по этой операции. |
| [GetWorksheet](./getworksheet/) | Получает рабочий лист. |
| [GetId](./getid/) | Получает номер этой ревизии. |
