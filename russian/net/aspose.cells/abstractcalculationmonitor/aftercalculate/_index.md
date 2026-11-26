---
title: "AbstractCalculationMonitor.AfterCalculate"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод AbstractCalculationMonitor. Реализуйте этот метод для выполнения бизнес-логики после вычисления одной ячейки"
type: docs
url: /ru/net/aspose.cells/abstractcalculationmonitor/aftercalculate/
---
## AbstractCalculationMonitor.AfterCalculate method

Реализуйте этот метод для выполнения бизнес-логики после вычисления ячейки.

```csharp
public virtual void AfterCalculate(int sheetIndex, int rowIndex, int colIndex)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| sheetIndex | Int32 | Индекс листа, к которому относится ячейка. |
| rowIndex | Int32 | Индекс строки ячейки |
| colIndex | Int32 | Индекс столбца ячейки |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AbstractCalculationMonitorMethodAfterCalculateWithInt32Int32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Настройте примерные формулы
            worksheet.Cells["A1"].Formula = "=1+2";
            worksheet.Cells["A2"].Formula = "=A1*3";
            worksheet.Cells["B1"].Formula = "=NOW()"; // Volatile function

            CalculationOptions options = new CalculationOptions();
            var monitor = new CalculationMonitor();
            options.CalculationMonitor = monitor;

            try
            {
                workbook.CalculateFormula(options);
                Console.WriteLine("Calculation completed. Check cell values and console output.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Calculation error: {ex.Message}");
            }

            workbook.Save("AfterCalculateDemo.xlsx");
        }


        private class CalculationMonitor : AbstractCalculationMonitor
        {
            public override void AfterCalculate(int sheetIndex, int rowIndex, int colIndex)
            {
                Console.WriteLine($"Calculated cell (Sheet {sheetIndex}): Row {rowIndex}, Column {colIndex}");
                Console.WriteLine($"Value changed: {ValueChanged}, Original: {OriginalValue}, New: {CalculatedValue}");
                Console.WriteLine("----------------------------------");
            }
        }
    }
}
```

### См. также

* class [AbstractCalculationMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


