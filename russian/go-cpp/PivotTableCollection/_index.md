---
title: "Класс PivotTableCollection"
linktitle: "PivotTableCollection"
second_title: "Справочник API Aspose.Cells for Go через C++"
description: "Класс PivotTableCollection. Инкапсулирует объект, представляющий pivottablecollection в Go."
type: docs
weight: 200
url: /ru/go-cpp/pivottablecollection/
---

## PivotTableCollection class

Представляет коллекцию всех объектов PivotTable на указанном листе.

```go

type PivotTableCollection struct  {
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
| [Dispose](./dispose/) | Выполняет задачи, определённые приложением, связанные с освобождением, выпуском или сбросом неуправляемых ресурсов. |
| [Add_String_Int_Int](./add_string_int_int/) | Добавляет новую сводную таблицу в указанную строку и столбец листа с параметрами по умолчанию. |
| [Add_String_Int_Int_String_Bool_Bool](./add_string_int_int_string_bool_bool/) | Добавляет новую сводную таблицу с устаревшим макетом и стилем Excel 97-2003. |
| [Add_String_String_String_Bool_Bool](./add_string_string_string_bool_bool/) | Добавляет новую сводную таблицу. |
| [Add_PivotTable_String_String](./add_pivottable_string_string/) | Добавляет новую сводную таблицу на основе другой сводной таблицы. |
| [Add_PivotTable_Int_Int_String](./add_pivottable_int_int_string/) | Добавляет новую сводную таблицу на основе другой сводной таблицы. |
| [Add_stringArray_Bool_PivotPageFields_String_String](./add_stringarray_bool_pivotpagefields_string_string/) | Добавляет новый объект PivotTable в коллекцию с несколькими диапазонами консолидации в качестве источника данных. |
| [Add_stringArray_Bool_PivotPageFields_Int_Int_String](./add_stringarray_bool_pivotpagefields_int_int_string/) | Добавляет новый объект PivotTable в коллекцию с несколькими диапазонами консолидации в качестве источника данных. |
| [Get_Int](./get_int/) | Получает отчет сводной таблицы по индексу. |
| [Get_String](./get_string/) | Получает отчет сводной таблицы по имени сводной таблицы. |
| [Get_Int_Int](./get_int_int/) | Получает отчет сводной таблицы по позиции сводной таблицы. |
| [Clear](./clear/) | Очищает все сводные таблицы. |
| [Remove_PivotTable](./remove_pivottable/) | Удаляет указанную сводную таблицу и удаляет данные сводной таблицы. |
| [Remove_PivotTable_Bool](./remove_pivottable_bool/) | Удаляет указанную сводную таблицу. |
| [RemoveAt_Int](./removeat_int/) | Удаляет сводную таблицу по указанному индексу и удаляет данные сводной таблицы. |
| [RemoveAt_Int_Bool](./removeat_int_bool/) | Удаляет сводную таблицу по указанному индексу. |
| [GetCount](./getcount/) | Получает количество элементов, содержащихся в экземпляре. |
