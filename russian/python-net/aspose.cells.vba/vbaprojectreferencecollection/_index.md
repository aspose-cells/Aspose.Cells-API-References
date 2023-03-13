---
title: VbaProjectReferenceCollection класс
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 50
url: /ru/python-net/aspose.cells.vba/vbaprojectreferencecollection/
is_root: false
---
##  VbaProjectReferenceCollection класс
Представляет все ссылки проекта VBA.



Тип VbaProjectReferenceCollection предоставляет следующие члены:

###  Характеристики
| Свойство| Описание|
| :- | :- |
| [capacity](/cells/ru/python-net/aspose.cells.vba/vbaprojectreferencecollection/capacity) | Получает или задает количество элементов, которые может содержать список массивов.|


###  Методы
| Метод| Описание|
| :- | :- |
| [copy_to(array)](/cells/ru/python-net/aspose.cells.vba/vbaprojectreferencecollection/copy_to/#list) | Копирует весь список массивов в совместимый список одномерных массивов, начиная с начала целевого списка массивов.|
| [copy_to(index, array, array_index, count)](/cells/ru/python-net/aspose.cells.vba/vbaprojectreferencecollection/copy_to/#int-list-int-int) |Копирует диапазон элементов из списка массивов в совместимый список одномерных массивов, начиная с указанного индекса целевого списка массивов.|
| [index_of(item, index)](/cells/ru/python-net/aspose.cells.vba/vbaprojectreferencecollection/index_of/#VbaProjectReference-int) | Выполняет поиск указанного объекта и возвращает отсчитываемый от нуля индекс первого вхождения в диапазоне элементов в списке массивов, который простирается от указанного индекса до последнего элемента.|
| [index_of(item, index, count)](/cells/ru/python-net/aspose.cells.vba/vbaprojectreferencecollection/index_of/#VbaProjectReference-int-int) | Выполняет поиск указанного объекта и возвращает отсчитываемый от нуля индекс первого вхождения в диапазоне элементов в списке массивов, который начинается с указанного индекса и содержит указанное количество элементов.|
| [last_index_of(item)](/cells/ru/python-net/aspose.cells.vba/vbaprojectreferencecollection/last_index_of/#VbaProjectReference) | Выполняет поиск указанного объекта и возвращает отсчитываемый от нуля индекс последнего вхождения во всем списке массивов.|
| [last_index_of(item, index)](/cells/ru/python-net/aspose.cells.vba/vbaprojectreferencecollection/last_index_of/#VbaProjectReference-int) | Выполняет поиск указанного объекта и возвращает отсчитываемый от нуля индекс последнего вхождения в диапазоне элементов в списке массивов, который простирается от первого элемента до указанного индекса.|
| [last_index_of(item, index, count)](/cells/ru/python-net/aspose.cells.vba/vbaprojectreferencecollection/last_index_of/#VbaProjectReference-int-int) |Выполняет поиск указанного объекта и возвращает отсчитываемый от нуля индекс последнего вхождения в диапазоне элементов в списке массивов, который содержит указанное количество элементов и заканчивается указанным индексом.|
| [add_registered_reference(name, libid)](/cells/ru/python-net/aspose.cells.vba/vbaprojectreferencecollection/add_registered_reference/#str-str) | Добавьте ссылку на библиотеку типов автоматизации.|
| [add_control_refrernce(name, libid, twiddledlibid, extended_libid)](/cells/ru/python-net/aspose.cells.vba/vbaprojectreferencecollection/add_control_refrernce/#str-str-str-str) | Добавьте ссылку на библиотеку измененных типов и ее расширенную библиотеку типов.|
| [add_project_refrernce(name, absolute_libid, relative_libid)](/cells/ru/python-net/aspose.cells.vba/vbaprojectreferencecollection/add_project_refrernce/#str-str-str) | Добавляет ссылку на внешний проект VBA.|
| [binary_search(item)](/cells/ru/python-net/aspose.cells.vba/vbaprojectreferencecollection/binary_search/#VbaProjectReference) | Ищет элемент во всем отсортированном списке массивов, используя компаратор по умолчанию, и возвращает отсчитываемый от нуля индекс элемента.|



###  Пример

```python
from aspose.cells import Workbook

# Instantiating a Workbook object
workbook = Workbook()
#  Init VBA project.
vbaProject = workbook.vba_project
#  Add vba project reference
vbaProject.references.add_registered_reference("stdole", "*\\G{00020430-0000-0000-C000-000000000046}#2.0#0#C:\\Windows\\system32\\stdole2.tlb#OLE Automation")
# Saving the Excel file
workbook.save("book1.xlsm")

```

###  Смотрите также
* модуль [aspose.cells.vba](..)
