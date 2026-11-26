---
title: "CalculationOptions.Recursive"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство CalculationOptions. Указывает, следует ли вычислять зависимые ячейки рекурсивно при расчёте одной ячейки, если она зависит от других ячеек. Значение по умолчанию — true"
type: docs
url: /ru/net/aspose.cells/calculationoptions/recursive/
---
## CalculationOptions.Recursive property

Указывает, следует ли вычислять зависимые ячейки рекурсивно при расчете одной ячейки, если она зависит от других ячеек. Значение по умолчанию — true.

```csharp
public bool Recursive { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CalculationOptionsPropertyRecursiveDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;
            
            // Создайте циклическую ссылку
            cells["A1"].Formula = "=A2";
            cells["A2"].Formula = "=A1";

            // Первое вычисление с Recursive=true (по умолчанию)
            CalculationOptions copts = new CalculationOptions();
            copts.Recursive = true;
            wb.CalculateFormula(copts);
            Console.WriteLine("Recursive calculation result (A2): " + cells["A2"].Value);

            // Второе вычисление с Recursive=false
            copts.Recursive = false;
            wb.CalculateFormula(copts);
            Console.WriteLine("Non-recursive calculation result (A2): " + cells["A2"].Value);
        }
    }
}
```

### См. также

* class [CalculationOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


