---
title: "ChartFrame.DefaultX"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ChartFrame. Представляет x позиции по умолчанию в единицах 1/4000 области диаграммы"
type: docs
url: /ru/net/aspose.cells.charts/chartframe/defaultx/
---
## ChartFrame.DefaultX property

Представляет x позиции по умолчанию в единицах 1/4000 области диаграммы.

```csharp
[Obsolete("Use ChartFrame.DefaultXRatioToChart property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int DefaultX { get; }
```

### Примечания

ПРИМЕЧАНИЕ: Этот член теперь устарел. Пожалуйста, используйте свойство ChartFrame.DefaultXRatioToChart вместо него. DefaultX = (int)(DefaultXRatioToChart * 4000); Это свойство будет удалено через 12 месяцев, начиная с февраля 2025 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartFramePropertyDefaultXDemo
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
            
            // Отобразить позицию X по умолчанию заголовка диаграммы
            Console.WriteLine("Default X position (1/4000 of chart area): " + chart.Title.DefaultX);
            Console.WriteLine("Default X position (ratio of chart area): " + chart.Title.DefaultXRatioToChart);
            
            // Показать, как позиция по умолчанию влияет на диаграмму
            Console.WriteLine("Is default position set? " + chart.Title.IsDefaultPosBeSet);
            
            // Изменить позицию заголовка, используя свойства отношения (поскольку DefaultX только для чтения)
            chart.Title.XRatioToChart = 0.2;
            chart.Title.YRatioToChart = 0.05;
            
            // Сохраните книгу
            workbook.Save("ChartFrameDefaultXDemo.xlsx");
        }
    }
}
```

### См. также

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


