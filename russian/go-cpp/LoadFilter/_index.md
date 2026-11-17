---
title: "Класс LoadFilter"
linktitle: "LoadFilter"
second_title: "Справочник API Aspose.Cells for Go через C++"
description: "Класс LoadFilter. Инкапсулирует объект, представляющий loadfilter в Go."
type: docs
weight: 200
url: /ru/go-cpp/loadfilter/
---

## LoadFilter class

Представляет фильтр, который предоставляет параметры загрузки данных при загрузке рабочей книги из шаблона.

```go

type LoadFilter struct  {
	ptr unsafe.Pointer
}

```
## Конструкторы

| Метод | Описание |
| --- | --- |
| [NewLoadFilter](./newloadfilter/) | Создаёт один LoadFilter с параметрами фильтра по умолчанию LoadDataFilterOptions::All. |
| [NewLoadFilter_LoadDataFilterOptions](./newloadfilter_loaddatafilteroptions/) | Создаёт один LoadFilter с заданными параметрами фильтра. |

## Методы

| Метод | Описание |
| --- | --- |
| [IsNull](./isnull/) | Проверяет, является ли объект реализации nullptr. |
| [GetLoadDataFilterOptions](./getloaddatafilteroptions/) | Получает параметры фильтра, указывающие, какие данные должны быть загружены. |
| [SetLoadDataFilterOptions](./setloaddatafilteroptions/) | Устанавливает параметры фильтра, указывающие, какие данные должны быть загружены. |
| [GetSheetsInLoadingOrder](./getsheetsinloadingorder/) | Указывает листы (индексы) и порядок их загрузки. По умолчанию значение null, что означает загрузку всех листов в порядке по умолчанию из шаблонного файла. Если не null и индекс какого‑то листа отсутствует в возвращённом массиве, то этот лист не будет загружен. |
| [StartSheet](./startsheet/) | Подготавливает параметры фильтра перед загрузкой указанного листа. Реализация LoadFilter пользователем может изменить LoadDataFilterOptions, указывая, как загружать данные для этого листа. |
