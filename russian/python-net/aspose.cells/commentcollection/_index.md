---
title: CommentCollection класс
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 290
url: /ru/python-net/aspose.cells/commentcollection/
is_root: false
---
##  CommentCollection класс
Инкапсулирует коллекцию из [Comment](/cells/ru/python-net/aspose.cells/comment) объектов.



Тип CommentCollection предоставляет следующие члены:

###  Характеристики
| Свойство| Описание|
| :- | :- |
| [capacity](/cells/ru/python-net/aspose.cells/commentcollection/capacity) | Получает или задает количество элементов, которые может содержать список массивов.|


###  Методы
| Метод| Описание|
| :- | :- |
| [add_threaded_comment(row, column, text, author)](/cells/ru/python-net/aspose.cells/commentcollection/add_threaded_comment/#int-int-str-ThreadedCommentAuthor) | Добавляет цепочку комментариев.|
| [add_threaded_comment(cell_name, text, author)](/cells/ru/python-net/aspose.cells/commentcollection/add_threaded_comment/#str-str-ThreadedCommentAuthor) | Добавляет цепочку комментариев.|
| [get_threaded_comments(row, column)](/cells/ru/python-net/aspose.cells/commentcollection/get_threaded_comments/#int-int) | Получает цепочку комментариев по индексу строки и столбца.|
| [get_threaded_comments(cell_name)](/cells/ru/python-net/aspose.cells/commentcollection/get_threaded_comments/#str) | Получает цепочку комментариев по имени ячейки.|
| [add(row, column)](/cells/ru/python-net/aspose.cells/commentcollection/add/#int-int) | Добавляет комментарий к коллекции.|
| [add(cell_name)](/cells/ru/python-net/aspose.cells/commentcollection/add/#str) | Добавляет комментарий к коллекции.|
| [remove_at(cell_name)](/cells/ru/python-net/aspose.cells/commentcollection/remove_at/#str) | Удаляет комментарий конкретной ячейки.|
| [remove_at(row, column)](/cells/ru/python-net/aspose.cells/commentcollection/remove_at/#int-int) | Удаляет комментарий конкретной ячейки.|
| [copy_to(array)](/cells/ru/python-net/aspose.cells/commentcollection/copy_to/#list) | Копирует весь список массивов в совместимый список одномерных массивов, начиная с начала целевого списка массивов.|
| [copy_to(index, array, array_index, count)](/cells/ru/python-net/aspose.cells/commentcollection/copy_to/#int-list-int-int) |Копирует диапазон элементов из списка массивов в совместимый список одномерных массивов, начиная с указанного индекса целевого списка массивов.|
| [index_of(item, index)](/cells/ru/python-net/aspose.cells/commentcollection/index_of/#Comment-int) | Выполняет поиск указанного объекта и возвращает отсчитываемый от нуля индекс первого вхождения в диапазоне элементов в списке массивов, который простирается от указанного индекса до последнего элемента.|
| [index_of(item, index, count)](/cells/ru/python-net/aspose.cells/commentcollection/index_of/#Comment-int-int) | Выполняет поиск указанного объекта и возвращает отсчитываемый от нуля индекс первого вхождения в диапазоне элементов в списке массивов, который начинается с указанного индекса и содержит указанное количество элементов.|
| [last_index_of(item)](/cells/ru/python-net/aspose.cells/commentcollection/last_index_of/#Comment) | Выполняет поиск указанного объекта и возвращает отсчитываемый от нуля индекс последнего вхождения во всем списке массивов.|
| [last_index_of(item, index)](/cells/ru/python-net/aspose.cells/commentcollection/last_index_of/#Comment-int) | Выполняет поиск указанного объекта и возвращает отсчитываемый от нуля индекс последнего вхождения в диапазоне элементов в списке массивов, который простирается от первого элемента до указанного индекса.|
| [last_index_of(item, index, count)](/cells/ru/python-net/aspose.cells/commentcollection/last_index_of/#Comment-int-int) |Выполняет поиск указанного объекта и возвращает отсчитываемый от нуля индекс последнего вхождения в диапазоне элементов в списке массивов, который содержит указанное количество элементов и заканчивается указанным индексом.|
| [binary_search(item)](/cells/ru/python-net/aspose.cells/commentcollection/binary_search/#Comment) | Ищет элемент во всем отсортированном списке массивов, используя компаратор по умолчанию, и возвращает отсчитываемый от нуля индекс элемента.|



###  Пример

```python
from aspose.cells import Workbook

workbook = Workbook()
comments = workbook.worksheets[0].comments

```

###  Смотрите также
* модуль [aspose.cells](..)
* класс [Comment](/cells/ru/python-net/aspose.cells/comment)
