---
title: "Chart.Is3D"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Chart. Указывает, является ли диаграмма 3D"
type: docs
url: /ru/net/aspose.cells.charts/chart/is3d/
---
## Chart.Is3D property

Указывает, является ли диаграмма 3‑D.

```csharp
public bool Is3D { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPropertyIs3DDemo
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
            worksheet.Cells["A5"].PutValue("Q4");

            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1200);
            worksheet.Cells["B3"].PutValue(1500);
            worksheet.Cells["B4"].PutValue(1800);
            worksheet.Cells["B5"].PutValue(2100);

            // Добавить столбчатую диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 6, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];

            // Установить диапазон данных для диаграммы
            chart.SetChartDataRange("A1:B5", true);

            // Отобразите текущее значение Is3D
            Console.WriteLine("Current Is3D value: " + chart.Is3D);

            // Создайте 3D-версию диаграммы
            int chart3DIndex = worksheet.Charts.Add(ChartType.Column3D, 6, 12, 20, 22);
            Chart chart3D = worksheet.Charts[chart3DIndex];
            chart3D.SetChartDataRange("A1:B5", true);

            // Отобразите значение Is3D 3D-диаграммы
            Console.WriteLine("3D Chart Is3D value: " + chart3D.Is3D);

            // Сохраните книгу
            workbook.Save("ChartPropertyIs3DDemo.xlsx");
        }
    }
}
```

### См. также

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


