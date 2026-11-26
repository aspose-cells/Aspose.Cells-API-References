---
title: "Cell.GetDependentsInCalculation"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Cell. Получает все ячейки, чей вычисленный результат зависит от этой ячейки"
type: docs
url: /ru/net/aspose.cells/cell/getdependentsincalculation/
---
## Cell.GetDependentsInCalculation method

Получает все ячейки, результат вычисления которых зависит от этой ячейки.

```csharp
public IEnumerator GetDependentsInCalculation(bool recursive)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| recursive | Boolean | Возвращает ли те зависимости, которые не ссылаются напрямую на эту ячейку, а ссылаются на другие листовые элементы этой ячейки |

### Возвращаемое значение

Перечислитель для перечисления всех зависимых (объекты Cell)

### Примечания

Чтобы использовать этот метод, убедитесь, что для рабочей книги установлено значение true параметра [`EnableCalculationChain`](../../formulasettings/enablecalculationchain/) и она полностью вычислена с этим параметром. Если в этой ячейке нет ссылок на формулы, будет возвращено null.

### Примеры

```csharp
using System;
using System.Collections;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetDependentsInCalculationWithBooleanDemo
    {
        public static void Run()
        {
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
        }
    }
}
```

### См. также

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


