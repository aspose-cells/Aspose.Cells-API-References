---
title: "Класс RowCollection"
linktitle: "RowCollection"
second_title: "Справочник API Aspose.Cells for Go через C++"
description: "Класс RowCollection. Инкапсулирует объект, представляющий rowcollection в Go."
type: docs
weight: 200
url: /ru/go-cpp/rowcollection/
---

## RowCollection class

Собирает объекты <see cref="Row"/> , представляющие отдельные строки в листе.

```go

type RowCollection struct  {
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
| [GetCount](./getcount/) | Получает количество строк в этой коллекции. |
| [GetEnumerator](./getenumerator/) | Получает перечислитель, который перебирает строки в этой коллекции |
| [GetEnumerator_Bool_Bool](./getenumerator_bool_bool/) | Получает перечислитель, который перебирает строки в этой коллекции |
| [GetRowByIndex](./getrowbyindex/) | Получает объект строки по позиции в списке. |
| [Get](./get/) | Получает объект Row по заданному индексу строки. Объект Row с указанным индексом будет создан, если он ранее не существовал. |
| [Clear](./clear/) | Очищает все строки и ячейки. |
| [RemoveAt](./removeat/) | Удаляет элемент строки в указанном индексе (позиции) в этой коллекции. |
