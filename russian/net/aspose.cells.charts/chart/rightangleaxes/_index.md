---
title: "Chart.RightAngleAxes"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Chart. Истина, если оси диаграммы находятся под прямым углом. Применяется только к 3D‑диаграммам, за исключением Column3D и 3D‑круговых диаграмм"
type: docs
url: /ru/net/aspose.cells.charts/chart/rightangleaxes/
---
## Chart.RightAngleAxes property

Истина, если оси диаграммы находятся под прямым углом. Применяется только к 3‑D диаграммам (за исключением Column3D и 3‑D круговых диаграмм).

```csharp
public bool RightAngleAxes { get; set; }
```

### Примечания

Если это свойство истинно, свойство Perspective игнорируется.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyRightAngleAxesDemo
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
            worksheet.Cells["B3"].PutValue(25);
            worksheet.Cells["B4"].PutValue(35);

            // Добавить 3D столбчатую диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Установить диапазон данных диаграммы
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Продемонстрировать свойство RightAngleAxes
            chart.RightAngleAxes = true;
            Console.WriteLine("RightAngleAxes is set to: " + chart.RightAngleAxes);

            // Сохраните книгу
            workbook.Save("RightAngleAxesDemo.xlsx");
        }
    }
}
```

### См. также

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


