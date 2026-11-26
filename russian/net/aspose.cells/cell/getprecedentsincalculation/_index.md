---
title: "Cell.GetPrecedentsInCalculation"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Cell. Возвращает все ссылки на предшествующие ячейки в текущей книге, используемые формулой этой ячейки при её вычислении."
type: docs
url: /ru/net/aspose.cells/cell/getprecedentsincalculation/
---
## Cell.GetPrecedentsInCalculation method

Получает все предшествующие (ссылки на ячейки в текущей книге), используемые формулой этой ячейки при её вычислении.

```csharp
public IEnumerator GetPrecedentsInCalculation()
```

### Возвращаемое значение

Перечислитель для перечисления всех ссылок (ReferredArea)

### Примечания

Этот метод может работать только в том случае, когда для книги установлен параметр [`EnableCalculationChain`](../../formulasettings/enablecalculationchain/) в значение true и книга полностью вычислена. Если эта ячейка не является формулой или не ссылается на другие ячейки, будет возвращено null.

### Примеры

```csharp
using System;
using System.Collections;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetPrecedentsInCalculationDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            cells["B1"].PutValue(10);
            cells["B2"].PutValue(20);
            cells["A2"].Formula = "=IF(TRUE,B2,B1)";
            
            workbook.Settings.FormulaSettings.EnableCalculationChain = true;
            workbook.CalculateFormula();
            
            IEnumerator en = cells["A2"].GetPrecedentsInCalculation();
            Console.WriteLine("A2's calculation precedents:");
            while(en.MoveNext())
            {
                ReferredArea r = (ReferredArea)en.Current;
                Console.WriteLine(r);
            }
        }
    }
}
```

### См. также

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


