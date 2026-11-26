---
title: "ChartFrame.DefaultY"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ChartFrame. Представляет y координату положения по умолчанию в единицах 1/4000 области диаграммы"
type: docs
url: /ru/net/aspose.cells.charts/chartframe/defaulty/
---
## ChartFrame.DefaultY property

Представляет y координату положения по умолчанию в единицах 1/4000 области диаграммы.

```csharp
[Obsolete("Use ChartFrame.DefaultYRatioToChart property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int DefaultY { get; }
```

### Примечания

ПРИМЕЧАНИЕ: Этот член теперь устарел. Пожалуйста, используйте вместо него свойство ChartFrame.DefaultYRatioToChart. DefaultY = (int)(DefaultYRatioToChart * 4000); Это свойство будет удалено через 12 месяцев, начиная с февраля 2025. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartFramePropertyDefaultYDemo
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
            
            // Установите источник данных диаграммы
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // Получить доступ к заголовку диаграммы, который наследуется от ChartFrame
            chart.Title.Text = "Sample Chart";
            ChartFrame chartFrame = chart.Title;
            
            // Отобразить текущее значение DefaultY (только для чтения)
            Console.WriteLine("DefaultY value (1/4000 of chart area): " + chartFrame.DefaultY);
            Console.WriteLine("DefaultY ratio to chart area: " + chartFrame.DefaultYRatioToChart);
            
            // Продемонстрировать, как DefaultY влияет на позиционирование, сравнив с текущим положением
            Console.WriteLine("Current Y position (ratio): " + chartFrame.YRatioToChart);
            
            // Сбросить позицию к значению по умолчанию с помощью SetPositionAuto()
            chartFrame.SetPositionAuto();
            Console.WriteLine("Y position after reset (ratio): " + chartFrame.YRatioToChart);
            
            // Сохранить результат
            workbook.Save("ChartFramePropertyDefaultYDemo.xlsx");
        }
    }
}
```

### См. также

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


