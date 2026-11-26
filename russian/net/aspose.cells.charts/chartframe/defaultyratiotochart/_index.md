---
title: "ChartFrame.DefaultYRatioToChart"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ChartFrame. Представляет y позиции по умолчанию в единицах доли области диаграммы"
type: docs
url: /ru/net/aspose.cells.charts/chartframe/defaultyratiotochart/
---
## ChartFrame.DefaultYRatioToChart property

Представляет y позиции по умолчанию в единицах доли области диаграммы.

```csharp
public double DefaultYRatioToChart { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartFramePropertyDefaultYRatioToChartDemo
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
            
            // Добавьте диаграмму и получите её кадр
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B4", true);
            
            // Получить chart frame (в данном случае заголовок)
            ChartFrame chartFrame = chart.Title;
            
            // Отобразить текущее значение DefaultYRatioToChart
            Console.WriteLine("Current DefaultYRatioToChart value: " + chartFrame.DefaultYRatioToChart);
            
            // Показать, как изменение YRatioToChart влияет на позицию (поскольку DefaultYRatioToChart только для чтения)
            Console.WriteLine("Current YRatioToChart value: " + chartFrame.YRatioToChart);
            chartFrame.YRatioToChart = 0.1; // Move title up
            Console.WriteLine("New YRatioToChart value: " + chartFrame.YRatioToChart);
            
            // Сохранить результат
            workbook.Save("PropertyDefaultYRatioToChartDemo.xlsx");
        }
    }
}
```

### См. также

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


