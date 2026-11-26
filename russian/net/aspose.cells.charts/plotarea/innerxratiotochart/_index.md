---
title: "PlotArea.InnerXRatioToChart"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PlotArea. Получает или получает координату x верхнего левого угла области построения в единицах отношения к области диаграммы"
type: docs
url: /ru/net/aspose.cells.charts/plotarea/innerxratiotochart/
---
## PlotArea.InnerXRatioToChart property

Получает или получает координату X верхнего угла области построения в единицах отношения к области диаграммы.

```csharp
public double InnerXRatioToChart { get; set; }
```

### Примечания

Ограничивающий прямоугольник области построения включает в себя область построения, деления (подписи делений) и небольшую границу вокруг делений. Если значение не создано в MS Excel, пожалуйста, вызовите метод Chart.Calculate() перед вызовом этого метода.

Значения **XRatioToChart**, **YRatioToChart**, **WidthRatioToChart** и **HeightRatioToChart** объекта **PlotArea** представляют ограничивающий прямоугольник области построения, который включает область построения, деления (метки делений) и небольшую границу вокруг делений. Если вы хотите получить фактический размер области построения, следует вызвать свойства **InnerXRatioToChart**, **InnerYRatioToChart**, **InnerWidthRatioToChart** и **InnerHeightRatioToChart**.

Для Excel 2007 или более новой версии значение по умолчанию равно нулю. Вы должны получить значение после вызова Chart.Calculate().

InnerX в пикселях = InnerXRatioToChart * chart.ChartObject.Width. Примечание: Когда задаётся InnerXRatioToChart, свойство IsInnerMode будет автоматически установлено в True.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class PlotAreaPropertyInnerXRatioToChartDemo
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
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Получить область построения диаграммы
            PlotArea plotArea = chart.PlotArea;

            // Отобразить текущее значение InnerXRatioToChart
            Console.WriteLine("Current InnerXRatioToChart value: " + plotArea.InnerXRatioToChart);

            // Установить новое значение для InnerXRatioToChart (смещение области построения вправо)
            plotArea.InnerXRatioToChart = 0.2;

            // Отобразить новое значение
            Console.WriteLine("New InnerXRatioToChart value: " + plotArea.InnerXRatioToChart);

            // Сохранить рабочую книгу, чтобы увидеть эффект
            workbook.Save("PlotAreaPropertyInnerXRatioToChartDemo.xlsx");
        }
    }
}
```

### См. также

* class [PlotArea](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


