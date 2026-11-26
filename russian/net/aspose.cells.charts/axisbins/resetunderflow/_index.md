---
title: "AxisBins.ResetUnderflow"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод AxisBins. Сбросить недополнение"
type: docs
url: /ru/net/aspose.cells.charts/axisbins/resetunderflow/
---
## AxisBins.ResetUnderflow method

Сбросить недополнение

```csharp
[Obsolete("This is an internal method.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void ResetUnderflow()
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

    public class AxisBinsMethodResetUnderflowDemo
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
            valueAxis.Bins.IsAutomatic = false;
            valueAxis.Bins.Count = 5;
            valueAxis.Bins.Underflow = 5;
            
            try
            {
                // Вызвать метод ResetUnderflow
                valueAxis.Bins.ResetUnderflow();
                
                Console.WriteLine("Underflow value after reset: " + valueAxis.Bins.Underflow);
                
                // Сохраните книгу
                workbook.Save("AxisBinsMethodResetUnderflowDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ResetUnderflow method: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [AxisBins](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


