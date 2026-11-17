---
title: "Класс PdfBookmarkEntry"
linktitle: "PdfBookmarkEntry"
second_title: "Справочник API Aspose.Cells for Go через C++"
description: "Класс PdfBookmarkEntry. Инкапсулирует объект, представляющий pdfbookmarkentry в Go."
type: docs
weight: 200
url: /ru/go-cpp/pdfbookmarkentry/
---

## PdfBookmarkEntry class

PdfBookmarkEntry является записью в закладках pdf. Если свойство Text текущего экземпляра равно null или "", текущий экземпляр будет скрыт, а дочерние элементы будут вставлены на текущий уровень.

```go

type PdfBookmarkEntry struct  {
	ptr unsafe.Pointer
}

```
## Конструкторы

| Метод | Описание |
| --- | --- |
| [NewPdfBookmarkEntry](./newpdfbookmarkentry/) | Конструктор по умолчанию. |

## Методы

| Метод | Описание |
| --- | --- |
| [IsNull](./isnull/) | Проверяет, является ли объект реализации nullptr. |
| [GetText](./gettext/) | Заголовок закладки. |
| [SetText](./settext/) | Заголовок закладки. |
| [GetDestination](./getdestination/) | Ячейка, к которой относится ссылка закладки. |
| [SetDestination](./setdestination/) | Ячейка, к которой относится ссылка закладки. |
| [GetDestinationName](./getdestinationname/) | Получает или задает имя назначения. |
| [SetDestinationName](./setdestinationname/) | Получает или задает имя назначения. |
| [IsOpen](./isopen/) | Если это свойство истинно, запись закладки будет расширяться, иначе она будет сворачиваться. |
| [SetIsOpen](./setisopen/) | Если это свойство истинно, запись закладки будет расширяться, иначе она будет сворачиваться. |
| [IsCollapse](./iscollapse/) | Если это свойство истинно, запись закладки будет сворачиваться, иначе она будет расширяться. |
| [SetIsCollapse](./setiscollapse/) | Если это свойство истинно, запись закладки будет сворачиваться, иначе она будет расширяться. |
