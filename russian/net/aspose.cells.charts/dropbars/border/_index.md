---
title: "DropBars.Border"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство DropBars. Получает границу Line"
type: docs
url: /ru/net/aspose.cells.charts/dropbars/border/
---
## DropBars.Border property

Получает границу [`Line`](../../../aspose.cells.drawing/line/).

```csharp
public Line Border { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class DropBarsPropertyBorderDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные для диаграммы
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);

            // Добавить линейную диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Добавьте серию данных в диаграмму
            chart.NSeries.Add("A1:B3", true);

            // Включить столбцы вверх/вниз
            chart.NSeries[0].HasUpDownBars = true;

            try
            {
                // Получить доступ к объектам DropBars
                DropBars upBars = chart.NSeries[0].UpBars;
                DropBars downBars = chart.NSeries[0].DownBars;

                // Отобразить текущие свойства границы (только для чтения)
                Console.WriteLine("Up Bars Border Color: " + upBars.Border.Color);
                Console.WriteLine("Up Bars Border Style: " + upBars.Border.Style);
                Console.WriteLine("Up Bars Border Weight: " + upBars.Border.WeightPt);
                Console.WriteLine("Up Bars Border Visibility: " + upBars.Border.IsVisible);

                Console.WriteLine("\nDown Bars Border Color: " + downBars.Border.Color);
                Console.WriteLine("Down Bars Border Style: " + downBars.Border.Style);
                Console.WriteLine("Down Bars Border Weight: " + downBars.Border.WeightPt);
                Console.WriteLine("Down Bars Border Visibility: " + downBars.Border.IsVisible);

                // Изменить свойства границы (поскольку Line не является только для чтения)
                upBars.Border.Color = Color.Blue;
                upBars.Border.Style = LineType.Solid;
                upBars.Border.WeightPt = 2.0;
                upBars.Border.IsVisible = true;

                downBars.Border.Color = Color.Red;
                downBars.Border.Style = LineType.Dash;
                downBars.Border.WeightPt = 1.5;
                downBars.Border.IsVisible = true;

                // Сохраните книгу
                workbook.Save("DropBarsBorderDemo.xlsx");
                Console.WriteLine("\nBorder properties have been demonstrated and saved to file.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [Line](../../../aspose.cells.drawing/line/)
* class [DropBars](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


