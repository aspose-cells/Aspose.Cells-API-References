---
title: update_linked_data_source метод
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 410
url: /ru/python-net/aspose.cells/workbook/update_linked_data_source/
is_root: false
---
##  update_linked_data_source(external_workbooks) {#list}
Если эта рабочая книга содержит внешние ссылки на другой источник данных,
Aspose.Cells попытается получить последние данные.



```python
def update_linked_data_source(self, external_workbooks):
    ...
```


| Параметр| Тип| Описание|
| :- | :- | :- |
| external_workbooks | list | Эта книга ссылается на внешние рабочие книги.<br/>Если он равен нулю, мы напрямую откроем внешние связанные файлы.<br/>Если это не ноль,<br/>мы сначала проверим, есть ли внешняя ссылка в массиве;<br/> если нет, мы снова откроем внешние связанные файлы.|
###  Примечания

Если метод не вызывается перед вычислением формул,
Aspose.Cells будет использовать предыдущую информацию (кэшированную в файле);
 Установите CellsHelper.StartupPath,CellsHelper.AltStartPath,CellsHelper.LibraryPath.
И, пожалуйста, установите Workbook.FilePath, если эта книга из потока,
в противном случае Aspose.Cells иногда не мог получить полный путь по внешней ссылке.


###  Смотрите также
* модуль [aspose.cells](../../)
* класс [Workbook](/cells/ru/python-net/aspose.cells/workbook)
