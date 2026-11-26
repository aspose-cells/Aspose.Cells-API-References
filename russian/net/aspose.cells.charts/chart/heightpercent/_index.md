---
title: "Chart.HeightPercent"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Chart. Возвращает или задаёт высоту 3D‑диаграммы в процентах от её ширины в диапазоне от 5 до 500 процентов"
type: docs
url: /ru/net/aspose.cells.charts/chart/heightpercent/
---
## Chart.HeightPercent property

Возвращает или задает высоту 3‑D диаграммы в процентах от ширины диаграммы (от 5 до 500 процентов).

```csharp
public int HeightPercent { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyHeightPercentDemo
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

            // Установите свойство HeightPercent (управляет высотой 3D‑диаграммы в процентах от её ширины)
            chart.HeightPercent = 150; // 150% of chart width

            // Сохраните книгу
            workbook.Save("ChartHeightPercentDemo.xlsx");

            Console.WriteLine("Chart with HeightPercent 150% created successfully.");
        }
    }
}
```

### См. также

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


