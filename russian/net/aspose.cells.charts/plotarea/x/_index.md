---
title: "PlotArea.X"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PlotArea. Получает или задаёт координату x верхнего левого угла ограничивающего прямоугольника области построения в единицах 1/4000 области диаграммы"
type: docs
url: /ru/net/aspose.cells.charts/plotarea/x/
---
## PlotArea.X property

Получает или задаёт координату x верхнего левого угла ограничивающего прямоугольника области построения в единицах 1/4000 области диаграммы.

```csharp
[Obsolete("Use PlotArea.XRatioToChart property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public override int X { get; set; }
```

### Примечания

Ограничивающий прямоугольник области построения включает в себя область построения, деления (подписи делений) и небольшую границу вокруг делений. Если значение не создано в MS Excel, пожалуйста, вызовите метод Chart.Calculate() перед вызовом этого метода.

Значения **X**, **Y**, **Width** и **Height** объекта **PlotArea** представляют ограничивающий прямоугольник области построения, который включает область построения, деления (метки делений) и небольшую границу вокруг делений. Если вы хотите получить фактический размер области построения, следует вызвать свойства **InnerXRatioToChart**, **InnerYRatioToChart**, **InnerWidthRatioToChart** и **InnerHeightRatioToChart**.

Для Excel 2007 или более новой версии значение по умолчанию равно нулю. Вы должны получить значение после вызова Chart.Calculate().

Примечание: Когда задаётся X, свойство IsInnerMode будет автоматически установлено в false.

ПРИМЕЧАНИЕ: Этот член теперь устарел. Пожалуйста, используйте свойство PlotArea.XRatioToChart. X = XRatioToChart * 4000. Это свойство будет удалено через 12 месяцев, начиная с февраля 2025 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class PlotAreaPropertyXDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
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

            // Добавить диаграмму в лист
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 10);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Установите источник данных диаграммы
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Установить свойства PlotArea
            chart.PlotArea.X = 100;  // Demonstrate X property usage
            chart.PlotArea.Y = 200;
            chart.PlotArea.Width = 1000;
            chart.PlotArea.Height = 800;

            // Сохраните книгу
            workbook.Save("PlotAreaPropertyXDemo_out.xlsx");
        }
    }
}
```

### См. также

* class [PlotArea](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


