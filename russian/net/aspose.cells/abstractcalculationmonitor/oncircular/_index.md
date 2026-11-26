---
title: "AbstractCalculationMonitor.OnCircular"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод AbstractCalculationMonitor. Реализуйте этот метод для выполнения бизнес-логики при вычислении формул с круговыми ссылками"
type: docs
url: /ru/net/aspose.cells/abstractcalculationmonitor/oncircular/
---
## AbstractCalculationMonitor.OnCircular method

Реализуйте этот метод для выполнения бизнес-логики при расчёте формул с круговыми ссылками.

```csharp
public virtual bool OnCircular(IEnumerator circularCellsData)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| circularCellsData | IEnumerator | IEnumerator с элементами [`CalculationCell`](../../calculationcell/) представляющими ячейки, зависящие от круговых ссылок. |

### Возвращаемое значение

Нужно ли движку формул вычислять эти ячейки в круговом режиме после этого вызова. True — позволить движку формул продолжить вычисления для них. False — позволить движку формул просто пометить эти ячейки как Calculated.

### Примечания

В реализации пользователь также может задать ожидаемое значение как рассчитанный результат для части/всех этих ячейк, чтобы движок формул не вычислял их рекурсивно.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Collections;

    public class AbstractCalculationMonitorMethodOnCircularDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создать сценарий круговой ссылки
            worksheet.Cells["A1"].Formula = "=B1";
            worksheet.Cells["B1"].Formula = "=A1";

            CalculationOptions options = new CalculationOptions();
            options.CalculationMonitor = new CircularReferenceMonitor();

            try
            {
                workbook.CalculateFormula(options);
                Console.WriteLine("Calculation completed. Check console for circular reference handling.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Calculation error: {ex.Message}");
            }

            workbook.Save("OnCircularDemo.xlsx");
        }

        private class CircularReferenceMonitor : AbstractCalculationMonitor
        {
            public override bool OnCircular(IEnumerator circularCellsData)
            {
                Console.WriteLine("Circular reference detected!");
                while (circularCellsData.MoveNext())
                {
                    Console.WriteLine($"Circular cell: {circularCellsData.Current}");
                }
                return true; // Continue calculation
            }
        }
    }
}
```

### См. также

* class [AbstractCalculationMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


