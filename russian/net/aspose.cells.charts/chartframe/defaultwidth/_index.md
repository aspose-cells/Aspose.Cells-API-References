---
title: "ChartFrame.DefaultWidth"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ChartFrame. Представляет ширину позиции по умолчанию в единицах 1/4000 области диаграммы"
type: docs
url: /ru/net/aspose.cells.charts/chartframe/defaultwidth/
---
## ChartFrame.DefaultWidth property

Представляет ширину позиции по умолчанию в единицах 1/4000 области диаграммы.

```csharp
[Obsolete("Use ChartFrame.DefaultWidthRatioToChart property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int DefaultWidth { get; }
```

### Примечания

ПРИМЕЧАНИЕ: Этот член теперь устарел. Пожалуйста, используйте свойство ChartFrame.DefaultWidthRatioToChart. DefaultWidth = (int)(DefaultWidthRatioToChart * 4000); Это свойство будет удалено через 12 месяцев, начиная с февраля 2025 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartFramePropertyDefaultWidthDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте примерные данные для диаграммы
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Item1");
            worksheet.Cells["A3"].PutValue("Item2");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);
            
            // Добавить диаграмму в лист
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 1, 15, 10);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Установите источник данных диаграммы
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";
            
            // Получите заголовок диаграммы (который наследуется от ChartFrame)
            Title title = chart.Title;
            
            // Отобразите ширину по умолчанию рамки диаграммы (в данном случае заголовок)
            Console.WriteLine("DefaultWidth of chart title: " + title.DefaultWidth);
            
            // Примечание: DefaultWidth только для чтения, поэтому мы не можем установить его
            // Мы можем только прочитать его, чтобы понять размеры по умолчанию
            
            // Продемонстрируйте, как это свойство влияет на диаграмму
            Console.WriteLine("IsDefaultPosBeSet: " + title.IsDefaultPosBeSet);
            Console.WriteLine("DefaultWidthRatioToChart: " + title.DefaultWidthRatioToChart);
            
            // Сохраните книгу
            workbook.Save("ChartFrameDefaultWidthDemo.xlsx");
        }
    }
}
```

### См. также

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


