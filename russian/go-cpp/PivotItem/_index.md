---
title: "PivotItem Класс"
linktitle: "PivotItem"
second_title: "Справочник API Aspose.Cells for Go через C++"
description: "PivotItem класс. Инкапсулирует объект, представляющий pivotitem в Go."
type: docs
weight: 200
url: /ru/go-cpp/pivotitem/
---

## PivotItem class

Представляет элемент в отчёте PivotField.

```go

type PivotItem struct  {
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
| [IsHidden](./ishidden/) | Получает и задает, скрыт ли pivot item. |
| [SetIsHidden](./setishidden/) | Получает и задает, скрыт ли pivot item. |
| [GetPosition](./getposition/) | Указание индекса этого элемента во всех PivotItems поля. |
| [SetPosition](./setposition/) | Указание индекса этого элемента во всех PivotItems поля. |
| [GetPositionInSameParentNode](./getpositioninsameparentnode/) | Указание позиционного индекса в PivotItems под тем же родительским узлом. |
| [SetPositionInSameParentNode](./setpositioninsameparentnode/) | Указание позиционного индекса в PivotItems под тем же родительским узлом. |
| [Move](./move/) | Перемещает элемент вверх или вниз |
| [IsDetailHidden](./isdetailhidden/) | Получает и задает, скрыты ли детали этого pivot item. |
| [SetIsDetailHidden](./setisdetailhidden/) | Получает и задает, скрыты ли детали этого pivot item. |
| [IsCalculatedItem](./iscalculateditem/) | Указывает, является ли этот pivot item вычисляемым элементом формулы. |
| [GetFormula](./getformula/) | Получает формулу этого вычисляемого элемента. Работает только когда этот элемент является вычисляемым. |
| [IsMissing](./ismissing/) | Указывает, был ли элемент удалён из источника данных. |
| [GetStringValue](./getstringvalue/) | Получает строковое значение pivot item. Если значение равно null, будет возвращено "" |
| [GetDoubleValue](./getdoublevalue/) | Получает двойное значение pivot item. Если значение равно null или не является числом, будет возвращено 0. |
| [GetDateTimeValue](./getdatetimevalue/) | Получает значение даты и времени pivot item. Если значение равно null, будет возвращено DateTime.MinValue. |
| [GetValue](./getvalue/) | Получает значение pivot item |
| [GetName](./getname/) | Получает имя pivot item. |
| [SetName](./setname/) | Получает имя pivot item. |
