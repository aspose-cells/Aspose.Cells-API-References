---
title: "Класс PivotCache"
linktitle: "PivotCache"
second_title: "Справочник API Aspose.Cells for Go через C++"
description: "Класс PivotCache. Инкапсулирует объект, представляющий pivotcache в Go."
type: docs
weight: 200
url: /ru/go-cpp/pivotcache/
---

## PivotCache class

Представляет кэш памяти для некоторых отчётов PivotTable.

```go

type PivotCache struct  {
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
| [GetMissingItemsLimit](./getmissingitemslimit/) | Получает и задает количество неиспользуемых элементов, допускаемых до их удаления. Это значение MUST быть больше -2 и меньше 1048577. PivotCacheMissingItemsLimitConst; |
| [SetMissingItemsLimit](./setmissingitemslimit/) | Получает и задает количество неиспользуемых элементов, допускаемых до их удаления. Это значение MUST быть больше -2 и меньше 1048577. PivotCacheMissingItemsLimitConst; |
| [Refresh_PivotTableRefreshOption](./refresh_pivottablerefreshoption/) | Обновляет данные из источника данных и вычисляет данные для представления всех pivottables, чей источник данных — этот pivot cache. |
| [Refresh](./refresh/) | Обновляет данные из источника данных и вычисляет данные для представления всех pivottables, чей источник данных — этот pivot cache. |
| [GetPivotTables](./getpivottables/) | Получает все сводные таблицы с этим pivot cache. |
| [Dispose](./dispose/) | Освободить все ресурсы. |
| [GetSourceType](./getsourcetype/) | Получает PivotTableSourceType. |
