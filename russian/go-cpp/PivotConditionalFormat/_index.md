---
title: "Класс PivotConditionalFormat"
linktitle: "PivotConditionalFormat"
second_title: "Справочник API Aspose.Cells for Go через C++"
description: "Класс PivotConditionalFormat. Инкапсулирует объект, представляющий pivotconditionalformat в Go."
type: docs
weight: 200
url: /ru/go-cpp/pivotconditionalformat/
---

## PivotConditionalFormat class

Представляет условие форматирования PivotTable в коллекции PivotFormatCondition.

```go

type PivotConditionalFormat struct  {
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
| [GetCellAreas](./getcellareas/) | Получает все области ячеек, к которым применяется этот условный формат. |
| [GetPivotAreas](./getpivotareas/) | Получает все области сводки. |
| [AddCellArea](./addcellarea/) | Добавляет область на основе представления сводной таблицы. |
| [ApplyTo](./applyto/) | Применяет условный формат к диапазону. Только для области данных. |
| [AddFieldArea_PivotFieldType_String](./addfieldarea_pivotfieldtype_string/) | Добавляет область поля сводки. |
| [AddFieldArea_PivotFieldType_PivotField](./addfieldarea_pivotfieldtype_pivotfield/) | Добавляет область поля сводки. |
| [GetFormatConditions](./getformatconditions/) | Получает условия для условного форматирования сводной таблицы. |
| [GetScopeType](./getscopetype/) | Получает и задает тип области для условного форматирования сводной таблицы. |
| [SetScopeType](./setscopetype/) | Получает и задает тип области для условного форматирования сводной таблицы. |
| [GetRuleType](./getruletype/) | Получает и задает тип правила для условного форматирования сводной таблицы. |
| [SetRuleType](./setruletype/) | Получает и задает тип правила для условного форматирования сводной таблицы. |
