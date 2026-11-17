---
title: "DrawObject Класс"
linktitle: "DrawObject"
second_title: "Справочник API Aspose.Cells for Go через C++"
description: "DrawObject class. Инкапсулирует объект, представляющий drawobject в Go."
type: docs
weight: 200
url: /ru/go-cpp/drawobject/
---

## DrawObject class

DrawObject будет инициализирован и возвращён при рендеринге.

```go

type DrawObject struct  {
	ptr unsafe.Pointer
}

```
## Конструкторы

| Метод | Описание |
| --- | --- |

## Методы

| Метод | Описание |
| --- | --- |
| [IsNull](./isnull/) | Проверяет, является ли объект реализации nullptr. |
| [GetCell](./getcell/) | Указывает объект Cell при рендеринге. Все свойства ячейки доступны. |
| [GetShape](./getshape/) | Указывает объект Shape при рендеринге. Все свойства Shape доступны. |
| [GetImageBytes](./getimagebytes/) | Указывает байты изображения отрендеренного Chart, Shape при рендеринге. |
| [GetType](./gettype/) | Указывает тип DrawObject. |
| [GetCurrentPage](./getcurrentpage/) | Указывает индекс страницы DrawObject. Индекс страницы начинается с нуля. Один лист содержит несколько страниц при рендеринге. |
| [GetTotalPages](./gettotalpages/) | Указывает общее количество страниц в текущем рендеринге. |
| [GetSheetIndex](./getsheetindex/) | Указывает текущий индекс листа DrawObject. |
