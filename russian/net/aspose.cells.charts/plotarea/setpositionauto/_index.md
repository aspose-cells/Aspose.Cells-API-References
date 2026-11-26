---
title: "PlotArea.SetPositionAuto"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод PlotArea. Установить позицию области построения в автоматический режим"
type: docs
url: /ru/net/aspose.cells.charts/plotarea/setpositionauto/
---
## PlotArea.SetPositionAuto method

Установить позицию области построения в автоматический режим

```csharp
public override void SetPositionAuto()
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class PlotAreaMethodSetPositionAutoDemo
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
            
            // Установите источник данных диаграммы
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            try
            {
                // Получить область построения диаграммы
                PlotArea plotArea = chart.PlotArea;
                
                // Сначала вручную задайте некоторые значения позиции, чтобы продемонстрировать эффект
                plotArea.XRatioToChart = 0.1;
                plotArea.YRatioToChart = 0.1;
                plotArea.WidthRatioToChart = 0.8;
                plotArea.HeightRatioToChart = 0.8;
                
                // Вызовите SetPositionAuto, чтобы сбросить позиционирование в автоматический режим
                plotArea.SetPositionAuto();
                
                Console.WriteLine("Plot area position has been set to automatic.");
                
                // Сохраните книгу, чтобы показать эффект
                workbook.Save("PlotAreaSetPositionAutoDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetPositionAuto method: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [PlotArea](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


