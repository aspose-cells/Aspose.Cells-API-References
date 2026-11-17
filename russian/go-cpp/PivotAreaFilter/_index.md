---
title: "PivotAreaFilter Класс"
linktitle: "PivotAreaFilter"
second_title: "Справочник API Aspose.Cells for Go через C++"
description: "PivotAreaFilter класс. Инкапсулирует объект, представляющий pivotareafilter в Go."
type: docs
weight: 200
url: /ru/go-cpp/pivotareafilter/
---

## PivotAreaFilter class

Представляет фильтр <see cref="PivotArea"/> для <see cref="PivotTable"/>.

```go

type PivotAreaFilter struct  {
	ptr unsafe.Pointer
}

```
## Конструкторы

| Метод | Описание |
| --- | --- |
| [NewPivotAreaFilter](./newpivotareafilter/) | Конструктор по умолчанию. |

## Методы

| Метод | Описание |
| --- | --- |
| [IsNull](./isnull/) | Проверяет, является ли объект реализации nullptr. |
| [IsSubtotalSet](./issubtotalset/) | Получает, какой промежуточный итог установлен для этого фильтра. |
| [SetSubtotals](./setsubtotals/) | Промежуточный итог для фильтра. |
| [GetFieldIndex](./getfieldindex/) | Получает индекс поля в исходных полях, к которому относится этот фильтр. Значение -2 указывает на поле значений. |
| [GetSelected](./getselected/) | Указывает, имеет ли это поле выделение. Работает только когда сводная таблица находится в режиме контурного просмотра. |
| [SetSelected](./setselected/) | Указывает, имеет ли это поле выделение. Работает только когда сводная таблица находится в режиме контурного просмотра. |
