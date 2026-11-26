---
title: "CalculationOptions.CalculationMonitor"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство CalculationOptions. Монитор для пользователя, позволяющий отслеживать прогресс вычисления формул"
type: docs
url: /ru/net/aspose.cells/calculationoptions/calculationmonitor/
---
## CalculationOptions.CalculationMonitor property

Монитор для пользователя, позволяющий отслеживать прогресс вычисления формул.

```csharp
public AbstractCalculationMonitor CalculationMonitor { get; set; }
```

### Примеры

```csharp
using System;
using System.Collections;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CalculationOptionsPropertyCalculationMonitorDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Установить несколько примерных формул
            worksheet.Cells["A1"].Formula = "=1+2";
            worksheet.Cells["A2"].Formula = "=A1*3";
            worksheet.Cells["A3"].Formula = "=SUM(A1:A2)";

            // Создать параметры вычисления с пользовательским монитором
            CalculationOptions options = new CalculationOptions();
            options.CalculationMonitor = new SampleCalculationMonitor();

            // Вычислять формулы с мониторингом
            workbook.CalculateFormula(options);

            // Вывести результаты
            Console.WriteLine("A1: " + worksheet.Cells["A1"].Value);
            Console.WriteLine("A2: " + worksheet.Cells["A2"].Value);
            Console.WriteLine("A3: " + worksheet.Cells["A3"].Value);
        }
    }

    public class SampleCalculationMonitor : AbstractCalculationMonitor
    {
        public override bool OnCircular(IEnumerator circularCellsData)
        {
            // Обрабатывать циклические ссылки при необходимости
            return base.OnCircular(circularCellsData);
        }

        public override void BeforeCalculate(int sheetIndex, int rowIndex, int columnIndex)
        {
            Console.WriteLine($"Before calculation: Sheet{sheetIndex}, Row{rowIndex}, Col{columnIndex}");
        }

        public override void AfterCalculate(int sheetIndex, int rowIndex, int columnIndex)
        {
            Console.WriteLine($"After calculation: Sheet{sheetIndex}, Row{rowIndex}, Col{columnIndex}");
        }
    }
}
```

### См. также

* class [AbstractCalculationMonitor](../../abstractcalculationmonitor/)
* class [CalculationOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


