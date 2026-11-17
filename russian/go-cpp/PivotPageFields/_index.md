---
title: "Класс PivotPageFields"
linktitle: "PivotPageFields"
second_title: "Справочник API Aspose.Cells for Go через C++"
description: "PivotPageFields class. Инкапсулирует объект, представляющий pivotpagefields в Go."
type: docs
weight: 200
url: /ru/go-cpp/pivotpagefields/
---

## PivotPageFields class

Представляет элементы страниц сводной таблицы, если источник данных сводной таблицы — диапазоны консолидации. Он может содержать не более 4 элементов.

```go

type PivotPageFields struct  {
	ptr unsafe.Pointer
}

```
## Конструкторы

| Метод | Описание |
| --- | --- |
| [NewPivotPageFields](./newpivotpagefields/) | Представляет элементы полей сводной страницы. |

## Методы

| Метод | Описание |
| --- | --- |
| [IsNull](./isnull/) | Проверяет, является ли объект реализации nullptr. |
| [AddPageField](./addpagefield/) | Добавляет поле страницы. |
| [GetPageFieldCount](./getpagefieldcount/) | Получает количество полей страницы. |
| [AddIdentify](./addidentify/) | Устанавливает, какая метка элемента в каждом поле страницы используется для идентификации диапазона данных. Длина pageItemIndex.Length должна быть равна PageFieldCount, поэтому, пожалуйста, сначала добавьте поле страницы. |
