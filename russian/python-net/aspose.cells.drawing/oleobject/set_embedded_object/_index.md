---
title: set_embedded_object метод
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 170
url: /ru/python-net/aspose.cells.drawing/oleobject/set_embedded_object/
is_root: false
---
##  set_embedded_object(link_to_file, object_data, source_file_name, display_as_icon, label) {#bool-bytes-str-bool-str}
Задает данные встроенного объекта.



```python
def set_embedded_object(self, link_to_file, object_data, source_file_name, display_as_icon, label):
    ...
```


| Параметр| Тип| Описание|
| :- | :- | :- |
| link_to_file | bool | Указывает, ссылается ли объект на файл. Если true, параметр objectData игнорируется.|
| object_data | bytes | Данные встроенного объекта.|
| source_file_name | str | Имя файла.|
| display_as_icon | bool | Указывает, отображается ли объект в виде значка.<br/> Если true, исходные данные изображения будут закрыты значком.|
| label | str | Метка значка. Работает, только если displayAsIcon имеет значение true.|


##  set_embedded_object(link_to_file, object_data, source_file_name, display_as_icon, label, update_icon) {#bool-bytes-str-bool-str-bool}
Задает данные встроенного объекта.



```python
def set_embedded_object(self, link_to_file, object_data, source_file_name, display_as_icon, label, update_icon):
    ...
```


| Параметр| Тип| Описание|
| :- | :- | :- |
| link_to_file | bool | Указывает, ссылается ли объект на файл. Если true, параметр objectData игнорируется.|
| object_data | bytes | Данные встроенного объекта.|
| source_file_name | str | Имя файла.|
| display_as_icon | bool | Указывает, отображается ли объект в виде значка.<br/> Если true, исходные данные изображения будут закрыты значком.|
| label | str | Метка значка. Работает, только если displayAsIcon имеет значение true.|
| update_icon | bool | Указывает, обновляется ли значок автоматически.|
###  Примечания

Поскольку Aspose может обновить встроенные значки всех файлов, поэтому лучше добавить правильный значок с `update_icon` как ложный.


###  Смотрите также

* модуль [aspose.cells.drawing](../../)
* класс [OleObject](/cells/ru/python-net/aspose.cells.drawing/oleobject)
