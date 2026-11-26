---
title: "Chart.Style"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Chart. Получает и задает встроенный стиль"
type: docs
url: /ru/net/aspose.cells.charts/chart/style/
---
## Chart.Style property

Получает и задает встроенный стиль.

```csharp
public int Style { get; set; }
```

### Примечания

Значение должно быть от 1 до 48. Вернуть -1, если не установлено.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyStyleDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные для диаграммы
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B4"].PutValue(30);

            // Добавьте диаграмму
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart1 = worksheet.Charts[chartIndex];
            chart1.NSeries.Add("B2:B4", false);
            chart1.NSeries.CategoryData = "A2:A4";

            // Создать другую диаграмму и скопировать стиль из первой диаграммы
            chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 10, 20, 18);
            Aspose.Cells.Charts.Chart chart2 = worksheet.Charts[chartIndex];
            chart2.NSeries.Add("B2:B4", false);
            chart2.NSeries.CategoryData = "A2:A4";
            
            // Продемонстрировать использование свойства Style
            chart2.Style = chart1.Style;

            // Сохраните книгу
            workbook.Save("ChartStyleDemo.xlsx");
        }
    }
}
```

### См. также

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


