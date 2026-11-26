---
title: "ChartFrame.YRatioToChart"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ChartFrame. Получает или задает координату y верхнего левого угла в единицах отношения области диаграммы"
type: docs
url: /ru/net/aspose.cells.charts/chartframe/yratiotochart/
---
## ChartFrame.YRatioToChart property

Получает или задает координату y верхнего левого угла в единицах отношения к области диаграммы.

```csharp
public virtual double YRatioToChart { get; set; }
```

### Примечания

Это дробное значение, его допустимый диапазон от 0 до 1. Как преобразовать единицы отношения в пиксели? `YPixel = YRatioToChart * Chart.ChartObject.Height;`

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartFramePropertyYRatioToChartDemo
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
            
            // Получить доступ к заголовку диаграммы, который наследуется от ChartFrame
            chart.Title.Text = "Sample Chart";
            
            // Отобразить текущее значение YRatioToChart
            Console.WriteLine("Current Title YRatioToChart value: " + chart.Title.YRatioToChart);
            
            // Измените позицию Y заголовка относительно области диаграммы
            chart.Title.YRatioToChart = 0.1; // 10% from top of chart area
            
            // Отобразить новое значение YRatioToChart
            Console.WriteLine("New Title YRatioToChart value: " + chart.Title.YRatioToChart);
            
            // Получите доступ к легенде, которая также наследуется от ChartFrame
            chart.Legend.Position = LegendPositionType.Top;
            
            // Отобразить текущее значение YRatioToChart для легенды
            Console.WriteLine("Current Legend YRatioToChart value: " + chart.Legend.YRatioToChart);
            
            // Измените позицию Y легенды относительно области диаграммы
            chart.Legend.YRatioToChart = 0.15; // 15% from top of chart area
            
            // Отобразить новое значение YRatioToChart для легенды
            Console.WriteLine("New Legend YRatioToChart value: " + chart.Legend.YRatioToChart);
            
            // Сохраните книгу
            workbook.Save("ChartFramePropertyYRatioToChartDemo.xlsx");
        }
    }
}
```

### См. также

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


