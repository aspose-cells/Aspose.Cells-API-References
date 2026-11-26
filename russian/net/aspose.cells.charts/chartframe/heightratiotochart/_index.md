---
title: "ChartFrame.HeightRatioToChart"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ChartFrame. Получает или задает высоту рамки в единицах отношения к области диаграммы"
type: docs
url: /ru/net/aspose.cells.charts/chartframe/heightratiotochart/
---
## ChartFrame.HeightRatioToChart property

Получает или задает высоту кадра в единицах отношения к области диаграммы.

```csharp
public virtual double HeightRatioToChart { get; set; }
```

### Примечания

Это дробное значение, его допустимый диапазон от 0 до 1. Как преобразовать единицы отношения в пиксели? HeightPixel = HeightRatioToChart * Chart.ChartObject.Height;

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartFramePropertyHeightRatioToChartDemo
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
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Установите источник данных диаграммы
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Получите заголовок диаграммы (который наследуется от ChartFrame)
            chart.Title.Text = "Sample Chart";
            ChartFrame titleFrame = chart.Title;

            // Отобразить текущее значение HeightRatioToChart
            Console.WriteLine("Current HeightRatioToChart value: " + titleFrame.HeightRatioToChart);

            // Установить новое соотношение высоты (0.1 = 10% от высоты диаграммы)
            titleFrame.HeightRatioToChart = 0.1;

            // Продемонстрировать эффект, сравнив до и после
            Console.WriteLine("Title height reduced to 10% of chart height");

            // Сохранить результат
            workbook.Save("PropertyHeightRatioToChartDemo.xlsx");
        }
    }
}
```

### См. также

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


