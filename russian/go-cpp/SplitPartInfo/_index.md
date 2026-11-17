---
title: "SplitPartInfo Класс"
linktitle: "SplitPartInfo"
second_title: "Справочник API Aspose.Cells for Go через C++"
description: "SplitPartInfo класс. Инкапсулирует объект, представляющий splitpartinfo в Go."
type: docs
weight: 200
url: /ru/go-cpp/splitpartinfo/
---

## SplitPartInfo class

Представляет информацию об одном входе/выходе для множественных входов/выходов, например текущей странице, которую нужно отобразить при преобразовании электронной таблицы в изображение.

```go

type SplitPartInfo struct  {
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
| [GetPartIndex](./getpartindex/) | Индекс текущей части в последовательности (0 based). -1 означает, что нет нескольких частей, поэтому результат одинарный. |
| [GetSheetIndex](./getsheetindex/) | Индекс листа, в котором находится текущая часть. -1 обозначает, что лист только один. |
| [GetSheetName](./getsheetname/) | Имя листа, в котором находится текущая часть. |
