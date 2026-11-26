---
title: "Area.Formatting"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Area. Представляет форматирование области"
type: docs
url: /ru/net/aspose.cells.drawing/area/formatting/
---
## Area.Formatting property

Представляет форматирование области.

```csharp
public FormattingType Formatting { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class AreaPropertyFormattingDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные для диаграммы
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Добавьте диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Установить диапазон данных диаграммы
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Получите доступ к области диаграммы и задайте форматирование
            ChartArea chartArea = chart.ChartArea;
            chartArea.Area.Formatting = FormattingType.None;

            // Сохраните книгу
            workbook.Save("AreaPropertyFormattingDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### См. также

* enum [FormattingType](../../../aspose.cells.charts/formattingtype/)
* class [Area](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


