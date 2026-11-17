---
title: "Класс DataBar"
linktitle: "DataBar"
second_title: "Справочник API Aspose.Cells for Go через C++"
description: "Класс DataBar. Инкапсулирует объект, представляющий databar в Go."
type: docs
weight: 200
url: /ru/go-cpp/databar/
---

## DataBar class

Опишите правило условного форматирования DataBar.Это правило условного форматирования отображает градиентную полосу данных в диапазоне ячеек.

```go

type DataBar struct  {
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
| [GetAxisColor](./getaxiscolor/) | Получает цвет оси для ячеек с условным форматированием в виде полос данных. |
| [SetAxisColor](./setaxiscolor/) | Получает цвет оси для ячеек с условным форматированием в виде полос данных. |
| [GetAxisPosition](./getaxisposition/) | Получает или задает положение оси полос данных, указанных правилом условного форматирования. |
| [SetAxisPosition](./setaxisposition/) | Получает или задает положение оси полос данных, указанных правилом условного форматирования. |
| [GetBarFillType](./getbarfilltype/) | Получает или задает способ заполнения полосы данных цветом. |
| [SetBarFillType](./setbarfilltype/) | Получает или задает способ заполнения полосы данных цветом. |
| [GetDirection](./getdirection/) | Получает или задает направление отображения полосы данных. |
| [SetDirection](./setdirection/) | Получает или задает направление отображения полосы данных. |
| [GetBarBorder](./getbarborder/) | Получает объект, определяющий границу полосы данных. |
| [GetNegativeBarFormat](./getnegativebarformat/) | Получает объект NegativeBarFormat, связанный с правилом условного форматирования полосы данных. |
| [GetMinCfvo](./getmincfvo/) | Получить или задать объект минимального значения этой DataBar. Нельзя установить null или CFValueObject с типом FormatConditionValueType.Max. |
| [GetMaxCfvo](./getmaxcfvo/) | Получить или задать объект максимального значения этой DataBar. Нельзя установить null или CFValueObject с типом FormatConditionValueType.Min. |
| [GetColor](./getcolor/) | Получить или задать цвет этой DataBar. |
| [SetColor](./setcolor/) | Получить или задать цвет этой DataBar. |
| [GetMinLength](./getminlength/) | Представляет минимальную длину полосы данных. |
| [SetMinLength](./setminlength/) | Представляет минимальную длину полосы данных. |
| [GetMaxLength](./getmaxlength/) | Представляет максимальную длину полосы данных. |
| [SetMaxLength](./setmaxlength/) | Представляет максимальную длину полосы данных. |
| [GetShowValue](./getshowvalue/) | Получить или задать флаг, указывающий, показывать ли значения ячеек, к которым применена эта полоса данных. Значение по умолчанию — true. |
| [SetShowValue](./setshowvalue/) | Получить или задать флаг, указывающий, показывать ли значения ячеек, к которым применена эта полоса данных. Значение по умолчанию — true. |
| [ToImage](./toimage/) | Отрисовать полосу данных в ячейке в массив байтов изображения. |
