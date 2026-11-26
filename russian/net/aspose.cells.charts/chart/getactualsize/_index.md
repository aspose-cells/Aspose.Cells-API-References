---
title: "Chart.GetActualSize"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Chart. Получает фактический размер диаграммы в пикселях."
type: docs
url: /ru/net/aspose.cells.charts/chart/getactualsize/
---
## Chart.GetActualSize method

Получает фактический размер диаграммы в пикселях.

```csharp
public int[] GetActualSize()
```

### Возвращаемое значение

Фактический размер в массиве (ширина и высота). [0] — ширина; [1] — высота.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartMethodGetActualSizeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте примерные данные для диаграммы
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            
            // Добавить диаграмму в лист
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Установить диапазон данных диаграммы
            chart.SetChartDataRange("A1:B4", true);
            
            try
            {
                // Вызовите метод GetActualSize.
                int[] actualSize = chart.GetActualSize();
                
                // Отобразить результат
                Console.WriteLine($"Actual chart size - Width: {actualSize[0]}px, Height: {actualSize[1]}px");
                
                // Покажите эффект, изменив размер объекта диаграммы.
                chart.ChartObject.Width = actualSize[0];
                chart.ChartObject.Height = actualSize[1];
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetActualSize method: {ex.Message}");
            }
            
            // Сохранить результат
            workbook.Save("ChartMethodGetActualSizeDemo.xlsx");
        }
    }
}
```

### См. также

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


