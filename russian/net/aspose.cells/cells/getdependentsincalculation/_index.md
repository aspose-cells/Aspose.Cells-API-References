---
title: GetDependentsInCalculation
second_title: Справочник по Aspose.Cells для .NET API
description: Получает все ячейки расчетный результат которых зависит от конкретной ячейки.
type: docs
weight: 710
url: /ru/net/aspose.cells/cells/getdependentsincalculation/
---
## Cells.GetDependentsInCalculation method

Получает все ячейки, расчетный результат которых зависит от конкретной ячейки.

```csharp
public IEnumerator GetDependentsInCalculation(int row, int column, bool recursive)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| row | Int32 | Индекс строки конкретной ячейки |
| column | Int32 | Индекс столбца конкретной ячейки. |
| recursive | Boolean | Возвращает ли те зависимые элементы, которые не ссылаются на конкретную ячейку напрямую , но ссылаются на другие листы этой ячейки. |

### Возвращаемое значение

Перечислитель для перечисления всех иждивенцев (объектов ячеек)

### Примечания

Чтобы использовать этот метод, убедитесь, что для рабочей книги задано истинное значение for [`EnableCalculationChain`](../../formulasettings/enablecalculationchain) и был полностью рассчитан с этой настройкой. Если в этой ячейке нет ссылки на формулу, будет возвращено значение null. Дополнительные сведения и пример см.[`GetDependentsInCalculation`](../../cell/getdependentsincalculation)

### Смотрите также

* class [Cells](../../cells)
* пространство имен [Aspose.Cells](../../cells)
* сборка [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
