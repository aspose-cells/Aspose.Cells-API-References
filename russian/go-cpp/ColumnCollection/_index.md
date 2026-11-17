---
title: "ColumnCollection Класс"
linktitle: "ColumnCollection"
second_title: "Справочник API Aspose.Cells for Go через C++"
description: "ColumnCollection класс. Инкапсулирует объект, представляющий columncollection в Go."
type: docs
weight: 200
url: /ru/go-cpp/columncollection/
---

## ColumnCollection class

Коллекция объектов <see cref="Column"/>, представляющих отдельные столбцы (настройки) в листе.Объект Column представляет только настройки, такие как ширина столбца, стили и т.д. для всего столбца, не имеет отношения к тому, есть ли непустые ячейки (данные) в соответствующем столбце. И "Count" этой коллекции представляет только количество объектов Column, созданных в этой коллекции, не имеет отношения к тому, есть ли непустые ячейки (данные) в листе.

```go

type ColumnCollection struct  {
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
| [GetColumnByIndex](./getcolumnbyindex/) | Получает объект Column по позиции в списке. |
| [Get](./get/) | Получает объект Column по индексу столбца.Объект Column заданного индекса столбца будет создан, если он ранее не существовал. |
| [GetCount](./getcount/) | Получает количество элементов, содержащихся в экземпляре. |
