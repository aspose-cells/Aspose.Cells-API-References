---
title: "ChartFrame.SetPositionAuto"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод ChartFrame. Установить позицию рамки в автоматический режим"
type: docs
url: /ru/net/aspose.cells.charts/chartframe/setpositionauto/
---
## ChartFrame.SetPositionAuto method

Установить позицию кадра в автоматический режим

```csharp
public virtual void SetPositionAuto()
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartFrameMethodSetPositionAutoDemo
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
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Установите источник данных диаграммы
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Получить рамку заголовка диаграммы
            ChartFrame title = chart.Title;
            
            // Сначала установить ручную позицию, чтобы продемонстрировать SetPositionAuto
            title.XRatioToChart = 0.2;
            title.YRatioToChart = 0.1;
            title.WidthRatioToChart = 0.6;
            title.HeightRatioToChart = 0.1;

            try
            {
                // Вызвать метод SetPositionAuto
                title.SetPositionAuto();
                
                Console.WriteLine("Chart title position set to automatic successfully");
                
                // Отобразить новые автоматические значения позиции
                Console.WriteLine($"New X position ratio: {title.XRatioToChart}");
                Console.WriteLine($"New Y position ratio: {title.YRatioToChart}");
                Console.WriteLine($"New Width ratio: {title.WidthRatioToChart}");
                Console.WriteLine($"New Height ratio: {title.HeightRatioToChart}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetPositionAuto method: {ex.Message}");
            }
            
            // Сохранить результат
            workbook.Save("ChartFrameSetPositionAutoDemo.xlsx");
        }
    }
}
```

### См. также

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


