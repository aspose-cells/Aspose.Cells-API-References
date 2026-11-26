---
title: "PlotArea.Height"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PlotArea. Получает или задает высоту ограничивающего прямоугольника области построения в единицах 1/4000 области диаграммы"
type: docs
url: /ru/net/aspose.cells.charts/plotarea/height/
---
## PlotArea.Height property

Получает или задает высоту ограничивающего прямоугольника области построения в единицах 1/4000 области диаграммы.

```csharp
[Obsolete("Use PlotArea.HeightRatioToChart property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public override int Height { get; set; }
```

### Примечания

Ограничивающий прямоугольник области построения включает в себя область построения, деления (подписи делений) и небольшую границу вокруг делений. Если значение не создано в MS Excel, пожалуйста, вызовите метод Chart.Calculate() перед вызовом этого метода.

Значения **X**, **Y**, **Width** и **Height** объекта **PlotArea** представляют ограничивающий прямоугольник области построения, который включает область построения, деления (метки делений) и небольшую границу вокруг делений. Если вы хотите получить фактический размер области построения, следует вызвать свойства **InnerXRatioToChart**, **InnerYRatioToChart**, **InnerWidthRatioToChart** и **InnerHeightRatioToChart**.

Для Excel 2007 или более новой версии значение по умолчанию равно нулю. Вы должны получить значение после вызова Chart.Calculate().

Примечание: Когда задаётся Height, свойство IsInnerMode будет автоматически установлено в false.

ПРИМЕЧАНИЕ: Этот член теперь устарел. Пожалуйста, используйте вместо него свойство PlotArea.HeightRatioToChart. Height = HeightRatioToChart * 4000. Это свойство будет удалено через 12 месяцев, начиная с февраля 2025 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class PlotAreaPropertyHeightDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные для диаграммы
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B4"].PutValue(30);

            // Добавьте диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Установите источник данных диаграммы
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Вычислить диаграмму
            chart.Calculate();

            // Продемонстрировать свойство Height
            Console.WriteLine("Chart Area Height: " + chart.ChartArea.Height);
            Console.WriteLine("Plot Area Height: " + chart.PlotArea.Height);

            // Изменить высоту PlotArea
            chart.PlotArea.Height = 2500;
            Console.WriteLine("Modified Plot Area Height: " + chart.PlotArea.Height);
        }
    }
}
```

### См. также

* class [PlotArea](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


