---
title: "GradientStop.Position"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство GradientStop. Позиция остановки"
type: docs
url: /ru/net/aspose.cells.drawing/gradientstop/position/
---
## GradientStop.Position property

Позиция остановки.

```csharp
public double Position { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class GradientStopPropertyPositionDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["B3"].PutValue(20);

            // Добавьте диаграмму
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = sheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B3", true);

            // Настроить градиентную заливку для первой серии
            Aspose.Cells.Charts.Series series = chart.NSeries[0];
            series.Area.FillFormat.FillType = Aspose.Cells.Drawing.FillType.Gradient;
            series.Area.FillFormat.GradientFill.SetPresetThemeGradient(
                Aspose.Cells.Drawing.PresetThemeGradientType.RadialGradient, 
                ThemeColorType.Accent1);

            // Получить доступ и изменить позиции градиентных остановок
            GradientStopCollection stops = series.Area.FillFormat.GradientFill.GradientStops;
            stops[0].Position = 0;
            stops[1].Position = 50;
            stops[2].Position = 100;

            // Сохраните книгу
            workbook.Save("GradientStopPositionDemo.xlsx");
        }
    }
}
```

### См. также

* class [GradientStop](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


