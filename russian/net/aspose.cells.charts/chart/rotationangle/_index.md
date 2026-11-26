---
title: "Chart.RotationAngle"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Chart. Представляет вращение 3D‑диаграммы, вращение области построения вокруг оси Z в градусах"
type: docs
url: /ru/net/aspose.cells.charts/chart/rotationangle/
---
## Chart.RotationAngle property

Представляет вращение 3‑D представления диаграммы (вращение области построения вокруг оси z в градусах).

```csharp
public int RotationAngle { get; set; }
```

### Примечания

Значение этого свойства должно быть от 0 до 360, за исключением 3‑D столбчатых диаграмм, где значение должно быть от 0 до 44. Значение по умолчанию — 20. Применяется только к 3‑D диаграммам.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyRotationAngleDemo
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

            // Добавить 3D столбчатую диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Установить диапазон данных диаграммы
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Установить угол вращения в 45 градусов
            chart.RotationAngle = 45;

            // Сохраните книгу
            workbook.Save("ChartRotationAngleDemo.xlsx");

            Console.WriteLine("Chart with rotation angle created successfully.");
        }
    }
}
```

### См. также

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


