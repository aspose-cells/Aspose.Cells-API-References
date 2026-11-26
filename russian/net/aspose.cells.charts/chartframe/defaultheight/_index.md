---
title: "ChartFrame.DefaultHeight"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ChartFrame. Представляет высоту позиции по умолчанию в единицах 1/4000 области диаграммы"
type: docs
url: /ru/net/aspose.cells.charts/chartframe/defaultheight/
---
## ChartFrame.DefaultHeight property

Представляет высоту позиции по умолчанию в единицах 1/4000 области диаграммы.

```csharp
[Obsolete("Use ChartFrame.DefaultHeightRatioToChart property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int DefaultHeight { get; }
```

### Примечания

ПРИМЕЧАНИЕ: Этот член теперь устарел. Пожалуйста, используйте свойство ChartFrame.DefaultHeightRatioToChart. DefaultHeight = (int)(DefaultHeightRatioToChart * 4000); Это свойство будет удалено через 12 месяцев, начиная с февраля 2025 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartFramePropertyDefaultHeightDemo
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

            // Получить доступ к заголовку диаграммы (который является ChartFrame)
            ChartFrame chartTitle = chart.Title;
            
            // Отобразить текущее значение DefaultHeight (свойство только для чтения)
            Console.WriteLine("Current DefaultHeight value: " + chartTitle.DefaultHeight);

            // Показать, как DefaultHeight влияет на макет диаграммы
            Console.WriteLine("DefaultHeightRatioToChart: " + chartTitle.DefaultHeightRatioToChart);
            Console.WriteLine("Current HeightRatioToChart: " + chartTitle.HeightRatioToChart);

            // Отрегулировать высоту, используя изменяемое свойство
            chartTitle.HeightRatioToChart = chartTitle.DefaultHeightRatioToChart * 1.5;
            Console.WriteLine("New HeightRatioToChart: " + chartTitle.HeightRatioToChart);

            // Сохранить результат
            workbook.Save("ChartFrameDefaultHeightDemo.xlsx");
        }
    }
}
```

### См. также

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


