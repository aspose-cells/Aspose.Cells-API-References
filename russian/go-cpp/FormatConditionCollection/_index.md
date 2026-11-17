---
title: "Класс FormatConditionCollection"
linktitle: "FormatConditionCollection"
second_title: "Справочник API Aspose.Cells for Go через C++"
description: "Класс FormatConditionCollection. Инкапсулирует объект, представляющий formatconditioncollection в Go."
type: docs
weight: 200
url: /ru/go-cpp/formatconditioncollection/
---

## FormatConditionCollection class

Представляет условное форматирование.ФорматУсловий может содержать до трех условных форматов.

```go

type FormatConditionCollection struct  {
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
| [Add](./add/) | Добавляет условие форматирования и затронутый диапазон ячеек в FormatConditions. FormatConditions могут содержать до трёх условных форматов. Ссылки на другие листы не допускаются в формулах условного форматирования. |
| [AddArea](./addarea/) | Добавляет диапазон ячеек с условным форматированием. |
| [AddCondition_FormatConditionType_OperatorType_String_String](./addcondition_formatconditiontype_operatortype_string_string/) | Добавляет условие форматирования. |
| [AddCondition_FormatConditionType](./addcondition_formatconditiontype/) | Добавьте условие формата. |
| [GetCount](./getcount/) | Возвращает количество условий. |
| [GetRangeCount](./getrangecount/) | Возвращает количество условно отформатированных диапазонов. |
| [Get](./get/) | Возвращает условие форматирования по индексу. |
| [GetCellArea](./getcellarea/) | Возвращает условно отформатированный диапазон ячеек по индексу. |
| [RemoveArea_Int](./removearea_int/) | Удаляет условно отформатированный диапазон ячеек по индексу. |
| [RemoveArea_Int_Int_Int_Int](./removearea_int_int_int_int/) | Удалить условное форматирование в диапазоне. |
| [RemoveCondition](./removecondition/) | Удаляет условие форматирования по индексу. |
