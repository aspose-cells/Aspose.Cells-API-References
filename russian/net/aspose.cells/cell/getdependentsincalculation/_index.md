---
title: GetDependentsInCalculation
second_title: Справочник по Aspose.Cells для .NET API
description: Получает все ячейки расчетный результат которых зависит от этой ячейки.
type: docs
weight: 390
url: /ru/net/aspose.cells/cell/getdependentsincalculation/
---
## Cell.GetDependentsInCalculation method

Получает все ячейки, расчетный результат которых зависит от этой ячейки.

```csharp
public IEnumerator GetDependentsInCalculation(bool recursive)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| recursive | Boolean | Возвращает ли те иждивенцы, которые не ссылаются на эту ячейку напрямую , но ссылаются на другие листы этой ячейки |

### Возвращаемое значение

Перечислитель для перечисления всех иждивенцев (объектов ячеек)

### Примечания

Чтобы использовать этот метод, убедитесь, что для рабочей книги задано истинное значение for [`EnableCalculationChain`](../../formulasettings/enablecalculationchain) и был полностью рассчитан с этой настройкой. Если в этой ячейке нет ссылки на формулу, будет возвращено значение null.

### Примеры

```csharp
[C#]

Workbook workbook = new Workbook();
Cells cells = workbook.Worksheets[0].Cells;
cells["A1"].Formula = "=B1+SUM(B1:B10)+[Book1.xls]Sheet1!B2";
cells["A2"].Formula = "=IF(TRUE,B2,B1)";
workbook.Settings.FormulaSettings.EnableCalculationChain = true;
workbook.CalculateFormula();
IEnumerator en = cells["B1"].GetDependentsInCalculation(false);
Console.WriteLine("B1's calculation dependents:");
while(en.MoveNext())
{
    Cell c = (Cell)en.Current;
    Console.WriteLine(c.Name);
}
en = cells["B2"].GetDependentsInCalculation(false);
Console.WriteLine("B2's calculation dependents:");
while(en.MoveNext())
{
    Cell c = (Cell)en.Current;
    Console.WriteLine(c.Name);
}
```

### Смотрите также

* class [Cell](../../cell)
* пространство имен [Aspose.Cells](../../cell)
* сборка [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
