---
title: "Класс AbstractCalculationMonitor"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.AbstractCalculationMonitor. Монитор для пользователя, позволяющий отслеживать прогресс вычисления формул"
type: docs
url: /ru/net/aspose.cells/abstractcalculationmonitor/
---
## AbstractCalculationMonitor class

Мониторинг для пользователя, позволяющий отслеживать прогресс вычисления формул.

```csharp
public abstract class AbstractCalculationMonitor
```

## Свойства

| Имя | Описание |
| --- | --- |
| [CalculatedValue](../../aspose.cells/abstractcalculationmonitor/calculatedvalue/) { get; } | Получает новое вычисленное значение ячейки. Должно использоваться только в [`AfterCalculate`](./aftercalculate/). |
| [OriginalValue](../../aspose.cells/abstractcalculationmonitor/originalvalue/) { get; } | Получает старое значение вычисленной ячейки. Должно использоваться только в [`BeforeCalculate`](./beforecalculate/) и [`AfterCalculate`](./aftercalculate/). |
| [ValueChanged](../../aspose.cells/abstractcalculationmonitor/valuechanged/) { get; } | Указывает, изменилось ли значение ячейки после вычисления. Должно использоваться только в [`AfterCalculate`](./aftercalculate/). |

## Методы

| Имя | Описание |
| --- | --- |
| virtual [AfterCalculate](../../aspose.cells/abstractcalculationmonitor/aftercalculate/)(int, int, int) | Реализуйте этот метод для выполнения бизнес-логики после вычисления ячейки. |
| virtual [BeforeCalculate](../../aspose.cells/abstractcalculationmonitor/beforecalculate/)(int, int, int) | Реализуйте этот метод для выполнения бизнес-логики перед вычислением ячейки. |
| virtual [OnCircular](../../aspose.cells/abstractcalculationmonitor/oncircular/)(IEnumerator) | Реализуйте этот метод для выполнения бизнес-логики при расчёте формул с круговыми ссылками. |

### Примеры

```csharp
using Aspose.Cells;
using System;
using System.Collections;

namespace AsposeCellsExamples
{
    // Пользовательская реализация AbstractCalculationMonitor
    public class CustomCalculationMonitor : AbstractCalculationMonitor
    {
        public override void BeforeCalculate(int sheetIndex, int rowIndex, int colIndex)
        {
            Console.WriteLine($"Before calculating cell at Sheet: {sheetIndex}, Row: {rowIndex}, Column: {colIndex}");
        }

        public override void AfterCalculate(int sheetIndex, int rowIndex, int colIndex)
        {
            Console.WriteLine($"After calculating cell at Sheet: {sheetIndex}, Row: {rowIndex}, Column: {colIndex}");
            Console.WriteLine($"Original Value: {OriginalValue}, Calculated Value: {CalculatedValue}, Value Changed: {ValueChanged}");
        }

        public override bool OnCircular(IEnumerator circularCellsData)
        {
            Console.WriteLine("Circular reference detected.");
            return false; // Return false to stop calculation when circular reference is detected
        }
    }

    public class CalculationMonitorDemo
    {
        public static void RunDemo()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Добавьте некоторые образцы данных.
            sheet.Cells["A1"].PutValue(10);
            sheet.Cells["A2"].PutValue(20);
            sheet.Cells["A3"].Formula = "=A1+A2";

            // Создайте экземпляр CustomCalculationMonitor
            CustomCalculationMonitor monitor = new CustomCalculationMonitor();

            // Установите параметры расчёта
            CalculationOptions options = new CalculationOptions
            {
                CalculationMonitor = monitor,
                IgnoreError = false,
                Recursive = true
            };

            // Вычислите формулы с пользовательским монитором
            workbook.CalculateFormula(options);

            // Сохраните книгу
            workbook.Save("CalculationMonitorDemo.xlsx");
            workbook.Save("CalculationMonitorDemo.pdf");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


