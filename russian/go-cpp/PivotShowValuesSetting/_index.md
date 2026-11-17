---
title: "Класс PivotShowValuesSetting"
linktitle: "PivotShowValuesSetting"
second_title: "Справочник API Aspose.Cells for Go через C++"
description: "Класс PivotShowValuesSetting. Инкапсулирует объект, представляющий pivotshowvaluessetting в Go."
type: docs
weight: 200
url: /ru/go-cpp/pivotshowvaluessetting/
---

## PivotShowValuesSetting class

Представляет настройки отображения значений, когда используется расчёт ShowDataAs.

```go

type PivotShowValuesSetting struct  {
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
| [GetCalculationType](./getcalculationtype/) | Представляет, как отображать значения поля данных в сводном отчёте. |
| [SetCalculationType](./setcalculationtype/) | Представляет, как отображать значения поля данных в сводном отчёте. |
| [GetBaseFieldIndex](./getbasefieldindex/) | Представляет базовое поле для вычисления ShowDataAs, когда вычисление ShowDataAs используется. |
| [SetBaseFieldIndex](./setbasefieldindex/) | Представляет базовое поле для вычисления ShowDataAs, когда вычисление ShowDataAs используется. |
| [GetBaseItemPositionType](./getbaseitempositiontype/) | Представляет тип базового элемента сводки в базовом поле, когда вычисление ShowDataAs используется. Действительно только для полей данных. Поскольку PivotItemPosition.Custom доступен только для чтения, если необходимо установить PivotItemPosition.Custom, пожалуйста, установите атрибут PivotField.BaseItemIndex. |
| [SetBaseItemPositionType](./setbaseitempositiontype/) | Представляет тип базового элемента сводки в базовом поле, когда вычисление ShowDataAs используется. Действительно только для полей данных. Поскольку PivotItemPosition.Custom доступен только для чтения, если необходимо установить PivotItemPosition.Custom, пожалуйста, установите атрибут PivotField.BaseItemIndex. |
| [GetBaseItemIndex](./getbaseitemindex/) | Представляет пользовательский индекс элемента сводки в базовом поле, когда вычисление ShowDataAs используется. Действительно только для полей данных. |
| [SetBaseItemIndex](./setbaseitemindex/) | Представляет пользовательский индекс элемента сводки в базовом поле, когда вычисление ShowDataAs используется. Действительно только для полей данных. |
