---
title: "Класс NameCollection"
linktitle: "NameCollection"
second_title: "Справочник API Aspose.Cells for Go через C++"
description: "Класс NameCollection. Инкапсулирует объект, представляющий namecollection в Go."
type: docs
weight: 200
url: /ru/go-cpp/namecollection/
---

## NameCollection class

Представляет коллекцию всех объектов <see cref=\"Name\"/> в электронной таблице.

```go

type NameCollection struct  {
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
| [Add](./add/) | Определяет новое имя. |
| [Get_Int](./get_int/) | Получает элемент Name по указанному индексу. |
| [Filter](./filter/) | Получает все определённые имена по области. |
| [Get_String](./get_string/) | Получает элемент Name с указанным именем. |
| [Remove_stringArray](./remove_stringarray/) | Удалить массив имён |
| [Remove_String](./remove_string/) | Удалить имя. |
| [RemoveAt](./removeat/) | Удалить имя по конкретному индексу. |
| [Clear](./clear/) | Удалить все определённые имена, которые не используются в формулах и источнике данных. Если определённое имя используется, мы только устанавливаем Name.ReferTo в null и скрываем их. |
| [RemoveDuplicateNames](./removeduplicatenames/) | Удалить дублирующие определённые имена |
| [Sort](./sort/) | Сортирует определённые имена. |
| [GetCount](./getcount/) | Получает количество элементов, содержащихся в экземпляре. |
