---
title: "ChartFrame.WidthRatioToChart"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ChartFrame. Получает или задает ширину кадра в единицах отношения к области диаграммы"
type: docs
url: /ru/net/aspose.cells.charts/chartframe/widthratiotochart/
---
## ChartFrame.WidthRatioToChart property

Получает или задает ширину кадра в единицах отношения к области диаграммы.

```csharp
public virtual double WidthRatioToChart { get; set; }
```

### Примечания

Это дробное значение, его допустимый диапазон от 0 до 1. Как преобразовать единицы отношения в пиксели? WidthPixel = WidthRatioToChart * Chart.ChartObject.Width;

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartFramePropertyWidthRatioToChartDemo
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

            // Получить доступ к заголовку диаграммы, который является ChartFrame
            ChartFrame chartTitle = chart.Title;

            // Отобразить текущее соотношение ширины
            Console.WriteLine("Current WidthRatioToChart value: " + chartTitle.WidthRatioToChart);

            // Установить новое соотношение ширины (0.5 = 50% ширины диаграммы)
            chartTitle.WidthRatioToChart = 0.5;

            // Показать эффект, сохранив книгу
            workbook.Save("ChartFrameWidthRatioDemo.xlsx");

            Console.WriteLine("WidthRatioToChart property demonstrated successfully.");
        }
    }
}
```

### См. также

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


