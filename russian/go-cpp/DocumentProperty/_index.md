---
title: "Класс DocumentProperty"
linktitle: "DocumentProperty"
second_title: "Справочник API Aspose.Cells for Go через C++"
description: "Класс DocumentProperty. Инкапсулирует объект, представляющий documentproperty в Go."
type: docs
weight: 200
url: /ru/go-cpp/documentproperty/
---

## DocumentProperty class

Представляет пользовательское или встроенное свойство документа.

```go

type DocumentProperty struct  {
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
| [GetName](./getname/) | Возвращает имя свойства. |
| [GetValue](./getvalue/) | Получает или задает значение свойства. |
| [SetValue](./setvalue/) | Получает или задает значение свойства. |
| [IsLinkedToContent](./islinkedtocontent/) | Указывает, связано ли это свойство с содержимым |
| [GetSource](./getsource/) | Источник связанного содержимого. |
| [GetType](./gettype/) | Получает тип данных свойства. |
| [IsGeneratedName](./isgeneratedname/) | Возвращает true, если у этого свойства нет имени в хранилище OLE2, и уникальное имя было сгенерировано только для публичного API. |
| [ToString](./tostring/) | Возвращает значение свойства как строку. |
| [ToInt](./toint/) | Возвращает значение свойства как целое число. |
| [ToDouble](./todouble/) | Возвращает значение свойства как double. |
| [ToDateTime](./todatetime/) | Возвращает значение свойства как DateTime в локальном часовом поясе. |
| [ToBool](./tobool/) | Возвращает значение свойства как bool. |
