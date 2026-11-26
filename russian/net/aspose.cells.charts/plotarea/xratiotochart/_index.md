---
title: "PlotArea.XRatioToChart"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PlotArea. Получает или задает координату x верхнего левого угла ограничивающего прямоугольника области построения как отношение к области диаграммы."
type: docs
url: /ru/net/aspose.cells.charts/plotarea/xratiotochart/
---
## PlotArea.XRatioToChart property

Получает или задает координату X верхнего левого угла ограничивающего прямоугольника области построения как отношение к области диаграммы.

```csharp
public override double XRatioToChart { get; set; }
```

### Примечания

Ограничивающий прямоугольник области построения включает в себя область построения, деления (подписи делений) и небольшую границу вокруг делений. Если значение не создано в MS Excel, пожалуйста, вызовите метод Chart.Calculate() перед вызовом этого метода.

Значения **XRatioToChart**, **YRatioToChart**, **WidthRatioToChart** и **HeightRatioToChart** объекта **PlotArea** представляют ограничивающий прямоугольник области построения, который включает область построения, деления (метки делений) и небольшую границу вокруг делений. Если вы хотите получить фактический размер области построения, следует вызвать свойства **InnerXRatioToChart**, **InnerYRatioToChart**, **InnerWidthRatioToChart** и **InnerHeightRatioToChart**.

Для Excel 2007 или более новой версии значение по умолчанию равно нулю. Вы должны получить значение после вызова Chart.Calculate().

XPixel = XRatioToChart * chart.ChartObject.Width. Примечание: При установке XRatioToChart свойство IsInnerMode будет автоматически установлено в false.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class PlotAreaPropertyXRatioToChartDemo
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
            chart.SetChartDataRange("A1:B4", true);

            // Получить область построения диаграммы
            PlotArea plotArea = chart.PlotArea;

            // Отобразите текущее значение XRatioToChart
            Console.WriteLine("Current XRatioToChart value: " + plotArea.XRatioToChart);

            // Измените значение XRatioToChart, чтобы переместить область построения по горизонтали
            plotArea.XRatioToChart = 0.2; // 20% from the left of the chart area

            // Отобразите новое значение XRatioToChart
            Console.WriteLine("New XRatioToChart value: " + plotArea.XRatioToChart);

            // Сохранить рабочую книгу, чтобы увидеть эффект
            workbook.Save("PlotAreaXRatioToChartDemo.xlsx");
        }
    }
}
```

### См. также

* class [PlotArea](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


