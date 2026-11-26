---
title: "PlotArea.InnerWidthRatioToChart"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PlotArea. Получает или задает ширину области построения в единицах отношения к области диаграммы"
type: docs
url: /ru/net/aspose.cells.charts/plotarea/innerwidthratiotochart/
---
## PlotArea.InnerWidthRatioToChart property

Получает или задает ширину области построения в единицах отношения к области диаграммы.

```csharp
public double InnerWidthRatioToChart { get; set; }
```

### Примечания

Ограничивающий прямоугольник области построения включает в себя область построения, деления (подписи делений) и небольшую границу вокруг делений. Если значение не создано в MS Excel, пожалуйста, вызовите метод Chart.Calculate() перед вызовом этого метода.

Значения **XRatioToChart**, **YRatioToChart**, **WidthRatioToChart** и **HeightRatioToChart** объекта **PlotArea** представляют ограничивающий прямоугольник области построения, который включает область построения, деления (метки делений) и небольшую границу вокруг делений. Если вы хотите получить фактический размер области построения, следует вызвать свойства **InnerXRatioToChart**, **InnerYRatioToChart**, **InnerWidthRatioToChart** и **InnerHeightRatioToChart**.

Для Excel 2007 или более новой версии значение по умолчанию равно нулю. Вы должны получить значение после вызова Chart.Calculate().

InnerWidth в пикселях = InnerXRatioToChart * chart.ChartObject.Width. Примечание: Когда устанавливается InnerWidthRatioToChart, свойство IsInnerMode будет автоматически установлено в True.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class PlotAreaPropertyInnerWidthRatioToChartDemo
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
            
            // Добавьте диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Установите источник данных диаграммы
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // Доступ к области построения
            PlotArea plotArea = chart.PlotArea;
            
            // Отобразить текущее значение InnerWidthRatioToChart
            Console.WriteLine("Current InnerWidthRatioToChart value: " + plotArea.InnerWidthRatioToChart);
            
            // Установить новое значение InnerWidthRatioToChart (0.5 означает 50 % ширины диаграммы)
            plotArea.InnerWidthRatioToChart = 0.5;
            
            // Показать эффект изменения
            Console.WriteLine("Plot area width changed to 50% of chart width");
            
            // Сохранить результат
            workbook.Save("PlotAreaPropertyInnerWidthRatioToChartDemo.xlsx");
        }
    }
}
```

### См. также

* class [PlotArea](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


