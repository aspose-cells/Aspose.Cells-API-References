---
title: "PlotArea.Y"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PlotArea. Возвращает или задает координату y верхнего угла ограничивающего прямоугольника области построения в единицах 1/4000 области диаграммы."
type: docs
url: /ru/net/aspose.cells.charts/plotarea/y/
---
## PlotArea.Y property

Возвращает или задает координату y верхнего угла ограничивающего прямоугольника области построения в единицах 1/4000 области диаграммы.

```csharp
[Obsolete("Use PlotArea.YRatioToChart property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public override int Y { get; set; }
```

### Примечания

Ограничивающий прямоугольник области построения включает в себя область построения, деления (подписи делений) и небольшую границу вокруг делений. Если значение не создано в MS Excel, пожалуйста, вызовите метод Chart.Calculate() перед вызовом этого метода.

Значения **X**, **Y**, **Width** и **Height** объекта **PlotArea** представляют ограничивающий прямоугольник области построения, который включает область построения, деления (метки делений) и небольшую границу вокруг делений. Если вы хотите получить фактический размер области построения, следует вызвать свойства **InnerXRatioToChart**, **InnerYRatioToChart**, **InnerWidthRatioToChart** и **InnerHeightRatioToChart**.

Для Excel 2007 или более новой версии значение по умолчанию равно нулю. Вы должны получить значение после вызова Chart.Calculate().

Примечание: Когда задаётся Y, свойство IsInnerMode будет автоматически установлено в false.

ПРИМЕЧАНИЕ: Этот член теперь устарел. Пожалуйста, используйте свойство PlotArea.YRatioToChart. Y = YRatioToChart * 4000. Это свойство будет удалено через 12 месяцев, начиная с февраля 2025 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class PlotAreaPropertyYDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Пример данных
            sheet.Cells["A1"].PutValue("Category 1");
            sheet.Cells["A2"].PutValue("Category 2");
            sheet.Cells["B1"].PutValue(100);
            sheet.Cells["B2"].PutValue(50);

            // Создать диаграмму
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 5, 20, 10);
            Chart chart = sheet.Charts[chartIndex];

            // Установите данные диаграммы
            chart.NSeries.Add("B1:B2", false);
            chart.NSeries.CategoryData = "A1:A2";

            // Настройка области построения
            chart.PlotArea.Width = 300;
            chart.PlotArea.Height = 200;
            chart.PlotArea.X = 100;
            chart.PlotArea.Y = 150; // Demonstrating Y property usage

            // Сохраните книгу
            workbook.Save("PlotAreaPropertyYDemo.xlsx");
        }
    }
}
```

### См. также

* class [PlotArea](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


