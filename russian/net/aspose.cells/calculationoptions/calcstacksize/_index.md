---
title: "CalculationOptions.CalcStackSize"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство CalculationOptions. Размер стека для рекурсивного расчёта ячеек. Значение по умолчанию — 200"
type: docs
url: /ru/net/aspose.cells/calculationoptions/calcstacksize/
---
## CalculationOptions.CalcStackSize property

Размер стека для рекурсивного расчёта ячеек. Значение по умолчанию — 200.

```csharp
public int CalcStackSize { get; set; }
```

### Примечания

Когда требуется рекурсивно вычислять большое количество ячеек в дереве зависимостей, в процессе расчёта может возникнуть StackOverflowException. В этом случае пользователь должен указать меньшее значение для этого свойства. Для такой ситуации пользователь должен определить подходящее значение свойства, исходя из реальных формул и данных. Однако слишком маленькое значение может привести к ухудшению производительности расчёта формул, а значение меньше 2 сделает невозможным вычисление формулы, зависящей от другой. Поэтому, если указанное значение меньше 2, оно будет сброшено до 2.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CalculationOptionsPropertyCalcStackSizeDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;

            // Настройте примерные формулы, требующие расчёта стека
            cells["A1"].PutValue(1);
            int last = 100;
            cells["B1"].Formula = "=SUM(A1:A" + last + ")";
            
            for (int i = 2; i <= last; i++)
            {
                cells["A" + i].Formula = "=A" + (i - 1) + "*1.1";
                cells["B" + i].Formula = "=B" + (i - 1) + "+A" + i;
            }

            // Выполнить расчёт с пользовательским размером стека
            wb.CalculateFormula(new CalculationOptions() { CalcStackSize = 50 });
            
            Console.WriteLine("Calculation completed with custom stack size");
        }
    }
}
```

### См. также

* class [CalculationOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


