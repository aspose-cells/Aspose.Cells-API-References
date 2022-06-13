---
title: GetPrecedentsInCalculation
second_title: Справочник по Aspose.Cells для .NET API
description: Получает все прецеденты ссылки на ячейки в текущей книге используемые формулой этой ячейки при ее вычислении.
type: docs
weight: 480
url: /ru/net/aspose.cells/cell/getprecedentsincalculation/
---
## Cell.GetPrecedentsInCalculation method

Получает все прецеденты (ссылки на ячейки в текущей книге), используемые формулой этой ячейки при ее вычислении.

```csharp
public IEnumerator GetPrecedentsInCalculation()
```

### Возвращаемое значение

Перечислитель для перечисления всех ссылок (ReferredArea)

### Примечания

Этот метод может работать только в ситуации, когда[`EnableCalculationChain`](../../formulasettings/enablecalculationchain) верно для рабочей книги и рабочая книга была полностью рассчитана. Если эта ячейка не является формулой или не ссылается ни на какие другие ячейки, будет возвращено значение null.

### Примеры

```csharp
[C#]

Workbook workbook = new Workbook();
Cells cells = workbook.Worksheets[0].Cells;
cells["A2"].Formula = "=IF(TRUE,B2,B1)";
IEnumerator en = cells["A2"].GetPrecedentsInCalculation();
while(en.MoveNext())
{
     ReferredArea r = (ReferredArea)en.Current;
     Console.WriteLine(r.SheetName + "!" + CellsHelper.CellIndexToName(r.StartRow, r.StartColumn));
}
```

### Смотрите также

* class [Cell](../../cell)
* пространство имен [Aspose.Cells](../../cell)
* сборка [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->