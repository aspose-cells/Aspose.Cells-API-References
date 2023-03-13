---
title: LoadFilter класс
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 1010
url: /ru/python-net/aspose.cells/loadfilter/
is_root: false
---
##  LoadFilter класс
Представляет фильтр, предоставляющий параметры для загрузки данных при загрузке книги из шаблона.



Тип LoadFilter предоставляет следующие члены:

###  Конструкторы
| Конструктор| Описание|
| :- | :- |
| [LoadFilter()](/cells/ru/python-net/aspose.cells/loadfilter/__init__/#) | Создает один LoadFilter с параметрами фильтра по умолчанию LoadDataFilterOptions.All.|
| [LoadFilter(opts)](/cells/ru/python-net/aspose.cells/loadfilter/__init__/#LoadDataFilterOptions) | Создает один LoadFilter с заданными параметрами фильтра.|


###  Характеристики
| Свойство| Описание|
| :- | :- |
| [load_data_filter_options](/cells/ru/python-net/aspose.cells/loadfilter/load_data_filter_options) | Параметры фильтра для обозначения того, какие данные должны быть загружены.|
| [sheets_in_loading_order](/cells/ru/python-net/aspose.cells/loadfilter/sheets_in_loading_order) | Указывает листы (индексы) и порядок загрузки.<br/>Значение по умолчанию — null, что означает загрузку всех листов в порядке по умолчанию в файле шаблона.<br/> Если не ноль и в возвращаемом массиве нет индекса листа, лист не будет загружен.|


###  Методы
| Метод| Описание|
| :- | :- |
| [start_sheet(sheet)](/cells/ru/python-net/aspose.cells/loadfilter/start_sheet/#Worksheet) | Подготавливает параметры фильтра перед загрузкой данного рабочего листа.<br/>Пользовательская реализация LoadFilter может изменить LoadDataFilterOptions здесь<br/> для обозначения того, как загружать данные для этого рабочего листа.|



###  Примечания

Пользователь может указать параметры фильтра или реализовать свой собственный LoadFilter, чтобы указать, как загружать данные.

###  Смотрите также
* модуль [aspose.cells](..)
