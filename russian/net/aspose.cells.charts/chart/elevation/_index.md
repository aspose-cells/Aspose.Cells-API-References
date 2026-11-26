---
title: "Chart.Elevation"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Chart. Представляет высоту (подъём) 3D‑диаграммы в градусах"
type: docs
url: /ru/net/aspose.cells.charts/chart/elevation/
---
## Chart.Elevation property

Представляет высоту просмотра 3‑D диаграммы в градусах.

```csharp
public int Elevation { get; set; }
```

### Примечания

Подъём диаграммы — это высота, под которой вы просматриваете диаграмму, в градусах. По умолчанию значение равно 15 для большинства типов диаграмм. Значение этого свойства должно быть от -90 до 90, за исключением 3‑D столбчатых диаграмм, где оно должно быть от 0 до 44.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyElevationDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные для диаграммы
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Q1");
            worksheet.Cells["A3"].PutValue("Q2");
            worksheet.Cells["A4"].PutValue("Q3");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["B4"].PutValue(3000);

            // Добавить 3D столбчатую диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Установить диапазон данных диаграммы
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Установить свойство elevation (угол в градусах)
            chart.Elevation = 30;
            
            // Сохраните книгу
            workbook.Save("ChartElevationDemo.xlsx");

            Console.WriteLine("Chart created with elevation set to 30 degrees.");
        }
    }
}
```

### См. также

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


