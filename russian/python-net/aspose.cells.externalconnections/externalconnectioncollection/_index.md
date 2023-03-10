---
title: ExternalConnectionCollection класс
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 60
url: /ru/python-net/aspose.cells.externalconnections/externalconnectioncollection/
is_root: false
---
##  ExternalConnectionCollection класс
Указывает коллекцию [ExternalConnection](/cells/ru/python-net/aspose.cells.externalconnections/externalconnection)



Тип ExternalConnectionCollection предоставляет следующие члены:

###  Характеристики
| Свойство| Описание|
| :- | :- |
| [capacity](/cells/ru/python-net/aspose.cells.externalconnections/externalconnectioncollection/capacity) | Получает или задает количество элементов, которые может содержать список массивов.|


###  Методы
| Метод| Описание|
| :- | :- |
| [copy_to(array)](/cells/ru/python-net/aspose.cells.externalconnections/externalconnectioncollection/copy_to/#list) | Копирует весь список массивов в совместимый список одномерных массивов, начиная с начала целевого списка массивов.|
| [copy_to(index, array, array_index, count)](/cells/ru/python-net/aspose.cells.externalconnections/externalconnectioncollection/copy_to/#int-list-int-int) |Копирует диапазон элементов из списка массивов в совместимый список одномерных массивов, начиная с указанного индекса целевого списка массивов.|
| [index_of(item, index)](/cells/ru/python-net/aspose.cells.externalconnections/externalconnectioncollection/index_of/#ExternalConnection-int) | Выполняет поиск указанного объекта и возвращает отсчитываемый от нуля индекс первого вхождения в диапазоне элементов в списке массивов, который простирается от указанного индекса до последнего элемента.|
| [index_of(item, index, count)](/cells/ru/python-net/aspose.cells.externalconnections/externalconnectioncollection/index_of/#ExternalConnection-int-int) | Выполняет поиск указанного объекта и возвращает отсчитываемый от нуля индекс первого вхождения в диапазоне элементов в списке массивов, который начинается с указанного индекса и содержит указанное количество элементов.|
| [last_index_of(item)](/cells/ru/python-net/aspose.cells.externalconnections/externalconnectioncollection/last_index_of/#ExternalConnection) | Выполняет поиск указанного объекта и возвращает отсчитываемый от нуля индекс последнего вхождения во всем списке массивов.|
| [last_index_of(item, index)](/cells/ru/python-net/aspose.cells.externalconnections/externalconnectioncollection/last_index_of/#ExternalConnection-int) | Выполняет поиск указанного объекта и возвращает отсчитываемый от нуля индекс последнего вхождения в диапазоне элементов в списке массивов, который простирается от первого элемента до указанного индекса.|
| [last_index_of(item, index, count)](/cells/ru/python-net/aspose.cells.externalconnections/externalconnectioncollection/last_index_of/#ExternalConnection-int-int) |Выполняет поиск указанного объекта и возвращает отсчитываемый от нуля индекс последнего вхождения в диапазоне элементов в списке массивов, который содержит указанное количество элементов и заканчивается указанным индексом.|
| [get_external_connection_by_id(conn_id)](/cells/ru/python-net/aspose.cells.externalconnections/externalconnectioncollection/get_external_connection_by_id/#int) | Получает элемент [ExternalConnection](/cells/ru/python-net/aspose.cells.externalconnections/externalconnection) с указанным идентификатором.|
| [binary_search(item)](/cells/ru/python-net/aspose.cells.externalconnections/externalconnectioncollection/binary_search/#ExternalConnection) | Ищет элемент во всем отсортированном списке массивов, используя компаратор по умолчанию, и возвращает отсчитываемый от нуля индекс элемента.|



###  Пример

```python
from aspose.cells import Workbook

wb = Workbook("connection.xlsx")
dataConns = wb.data_connections
dataConn = None
for i in range(len(dataConns)):
    dataConn = dataConns[i]
    # get external connection id
    print(dataConn.connection_id)

```

###  Смотрите также
* модуль [aspose.cells.externalconnections](..)
* класс [ExternalConnection](/cells/ru/python-net/aspose.cells.externalconnections/externalconnection)
