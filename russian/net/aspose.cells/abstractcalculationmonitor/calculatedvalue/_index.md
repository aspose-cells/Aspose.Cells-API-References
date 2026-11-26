---
title: "AbstractCalculationMonitor.CalculatedValue"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство AbstractCalculationMonitor. Возвращает новое вычисленное значение ячейки. Должно использоваться только в AfterCalculate"
type: docs
url: /ru/net/aspose.cells/abstractcalculationmonitor/calculatedvalue/
---
## AbstractCalculationMonitor.CalculatedValue property

Возвращает новое вычисленное значение ячейки. Должно использоваться только в [`AfterCalculate`](../aftercalculate/).

```csharp
public object CalculatedValue { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CustomCalculationMonitor : AbstractCalculationMonitor
    {
        public override void AfterCalculate(int sheetIndex, int rowIndex, int columnIndex)
        {
            if (ValueChanged)
            {
                Console.WriteLine($"Value changed from [{OriginalValue}] to [{CalculatedValue}]");
            }
        }
    }

    public class AbstractCalculationMonitorPropertyCalculatedValueDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Настройте цепочку вычислений
            worksheet.Cells["A1"].Formula = "=1+2";
            worksheet.Cells["A2"].Formula = "=A1*3";

            // Создайте и присоедините монитор
            CustomCalculationMonitor monitor = new CustomCalculationMonitor();
            CalculationOptions options = new CalculationOptions();
            options.CalculationMonitor = monitor;

            // Запустите вычисление, которое вызовет наш монитор
            workbook.CalculateFormula(options);

            // Измените значение, чтобы вызвать уведомление об изменении значения
            worksheet.Cells["A1"].Value = 5;
            workbook.CalculateFormula(options);
        }
    }
}
```

### См. также

* class [AbstractCalculationMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


