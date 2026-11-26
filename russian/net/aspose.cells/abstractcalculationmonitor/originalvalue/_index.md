---
title: "AbstractCalculationMonitor.OriginalValue"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство AbstractCalculationMonitor. Возвращает старое значение вычисленной ячейки. Должно использоваться только в BeforeCalculate и AfterCalculate"
type: docs
url: /ru/net/aspose.cells/abstractcalculationmonitor/originalvalue/
---
## AbstractCalculationMonitor.OriginalValue property

Возвращает старое значение вычисленной ячейки. Должно использоваться только в [`BeforeCalculate`](../beforecalculate/) и [`AfterCalculate`](../aftercalculate/).

```csharp
public object OriginalValue { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CustomCalculationMonitor1 : AbstractCalculationMonitor
    {
        public override void AfterCalculate(int sheetIndex, int rowIndex, int colIndex)
        {
            if (ValueChanged)
            {
                Console.WriteLine($"Value changed from [{OriginalValue}] to [{CalculatedValue}]");
            }
        }
    }

    public class AbstractCalculationMonitorPropertyOriginalValueDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Установите начальное значение
            worksheet.Cells["A1"].PutValue(10);
            
            // Добавьте формулу, которая изменит значение
            worksheet.Cells["A2"].Formula = "=A1*2";
            
            // Установите монитор вычислений
            CalculationOptions options = new CalculationOptions();
            options.CalculationMonitor = new CustomCalculationMonitor1();
            
            // Перерасчитайте формулы — это вызовет монитор
            workbook.CalculateFormula(options);
            
            // Измените исходное значение, чтобы продемонстрировать работу монитора
            worksheet.Cells["A1"].PutValue(20);
            workbook.CalculateFormula(options);
        }
    }
}
```

### См. также

* class [AbstractCalculationMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


