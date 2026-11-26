---
title: "Chart.BackWall"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Chart. Возвращает объект Walls, представляющий заднюю стенку 3D‑диаграммы"
type: docs
url: /ru/net/aspose.cells.charts/chart/backwall/
---
## Chart.BackWall property

Возвращает объект [`Walls`](../walls/) , представляющий заднюю стенку 3‑D диаграммы.

```csharp
public Walls BackWall { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPropertyBackWallDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные для диаграммы
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Q1");
            worksheet.Cells["A3"].PutValue("Q2");
            worksheet.Cells["A4"].PutValue("Q3");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1200);
            worksheet.Cells["B3"].PutValue(1500);
            worksheet.Cells["B4"].PutValue(1800);

            // Добавить 3D столбчатую диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Установить диапазон данных диаграммы
            chart.SetChartDataRange("A1:B4", true);

            // Убедитесь, что это 3D‑диаграмма
            if (chart.Is3D)
            {
                // Получите объект BackWall
                Walls backWall = chart.BackWall;

                // Отобразите некоторые свойства BackWall
                Console.WriteLine("BackWall properties:");
                Console.WriteLine("CenterX: " + backWall.CenterX);
                Console.WriteLine("CenterY: " + backWall.CenterY);
                Console.WriteLine("Width: " + backWall.Width);
                Console.WriteLine("Height: " + backWall.Height);

                // Отформатируйте BackWall
                backWall.FillFormat.SetOneColorGradient(
                    System.Drawing.Color.LightBlue, 
                    0.5, // Changed from GradientStyleType to double for degree parameter
                    Aspose.Cells.Drawing.GradientStyleType.Horizontal, 
                    1); // Changed from 0.5 to int for variant parameter

                // Установить свойства границы
                backWall.Border.Color = System.Drawing.Color.DarkBlue;
                backWall.Border.Weight = Aspose.Cells.Drawing.WeightType.MediumLine;
            }

            // Сохраните книгу
            workbook.Save("ChartPropertyBackWallDemo.xlsx");
        }
    }
}
```

### См. также

* class [Walls](../../walls/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


