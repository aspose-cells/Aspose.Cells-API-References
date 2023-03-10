---
title: register_add_in_function метод
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 170
url: /ru/python-net/aspose.cells/worksheetcollection/register_add_in_function/
is_root: false
---
##  register_add_in_function(id, function_name) {#int-str}
Добавляет функцию надстройки в книгу


###  Возвращает

URL-адрес файла надстройки, который содержит функции надстройки


```python
def register_add_in_function(self, id, function_name):
    ...
```


| Параметр| Тип| Описание|
| :- | :- | :- |
| id | int | ID данных, которые содержат дополнительные функции,<br/> можно получить по первому звонку [WorksheetCollection.register_add_in_function(add_in_file, function_name, lib)](/cells/ru/python-net/aspose.cells/worksheetcollection/register_add_in_function) для того же файла надстройки.|
| function_name | str | имя функции надстройки|


##  register_add_in_function(add_in_file, function_name, lib) {#str-str-bool}
Добавляет функцию надстройки в книгу


###  Возвращает

ID данных, которые содержат заданную функцию надстройки


```python
def register_add_in_function(self, add_in_file, function_name, lib):
    ...
```


| Параметр| Тип| Описание|
| :- | :- | :- |
| add_in_file | str | файл содержит функции надстройки|
| function_name | str | имя функции надстройки|
| lib | bool | находится ли данный файл надстройки в каталоге или подкаталоге библиотеки надстроек Workbook.<br/>Этот флаг вступает в силу и имеет значение, когда данный addInFile имеет относительный путь:<br/> Значение true означает, что путь относится к библиотеке надстроек, а значение false означает, что путь относится к этой книге.|



###  Смотрите также
* модуль [aspose.cells](../../)
* класс [WorksheetCollection](/cells/ru/python-net/aspose.cells/worksheetcollection)
