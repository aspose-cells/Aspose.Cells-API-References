---
title: "Класс PivotFieldCollection"
linktitle: "PivotFieldCollection"
second_title: "Справочник API Aspose.Cells for Go через C++"
description: "Класс PivotFieldCollection. Инкапсулирует объект, представляющий pivotfieldcollection в Go."
type: docs
weight: 200
url: /ru/go-cpp/pivotfieldcollection/
---

## PivotFieldCollection class

Представляет коллекцию всех объектов PivotField в разных областях сводной таблицы.

```go

type PivotFieldCollection struct  {
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
| [GetType](./gettype/) | Получает тип PivotFields. |
| [Get_Int](./get_int/) | Получает объект PivotField по указанному индексу. |
| [Get_String](./get_string/) | Получает объект PivotField по указанному имени. |
| [RemoveAt](./removeat/) | Удаляет поле по индексу. Только для областей filter, row, column, data. |
| [AddByBaseIndex](./addbybaseindex/) | Добавляет объект PivotField к указанному типу PivotFields. |
| [Add](./add/) | Добавляет объект PivotField к указанному типу PivotFields. |
| [Insert](./insert/) | Вставляет поле сводной таблицы по указанному индексу. |
| [Clear](./clear/) | Очистить все поля PivotFieldCollection. |
| [Remove](./remove/) | Удаляет поле из текущей области. |
| [Move](./move/) | Перемещает PivotField из текущей позиции в целевую позицию. |
| [GetCount](./getcount/) | Получает количество элементов, содержащихся в экземпляре. |
