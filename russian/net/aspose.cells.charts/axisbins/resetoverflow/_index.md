---
title: "AxisBins.ResetOverflow"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод AxisBins. Сбросить переполнение"
type: docs
url: /ru/net/aspose.cells.charts/axisbins/resetoverflow/
---
## AxisBins.ResetOverflow method

Сбросить переполнение

```csharp
[Obsolete("This is an internal method.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void ResetOverflow()
```

### Примечания

ПРИМЕЧАНИЕ: Этот метод теперь устарел. Это внутренний метод, который не нужно вызывать извне, чтобы избежать проблем. Это свойство будет удалено через 12 месяцев, начиная с июля 2024 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class AxisBinsMethodResetOverflowDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные для диаграммы
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Создать диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Получить ось значений
            Axis valueAxis = chart.ValueAxis;

            // Создать корзины оси
            AxisBins bins = valueAxis.Bins;

            // Установить значение переполнения
            bins.Overflow = 25;
            Console.WriteLine($"Overflow before reset: {bins.Overflow}");

            try
            {
                // Вызвать метод ResetOverflow
                bins.ResetOverflow();
                Console.WriteLine($"Overflow after reset: {bins.Overflow}");
                Console.WriteLine("ResetOverflow method executed successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ResetOverflow method: {ex.Message}");
            }

            // Сохранить результат
            workbook.Save("AxisBinsMethodResetOverflowDemo.xlsx");
        }
    }
}
```

### См. также

* class [AxisBins](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


