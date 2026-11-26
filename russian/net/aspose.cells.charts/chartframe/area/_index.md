---
title: "ChartFrame.Area"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ChartFrame. Получает область"
type: docs
url: /ru/net/aspose.cells.charts/chartframe/area/
---
## ChartFrame.Area property

Получает `area`.

```csharp
public virtual Area Area { get; }
```

### Примеры

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ChartFramePropertyAreaDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Добавьте примерные данные для диаграммы
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["A4"].PutValue("C");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["B3"].PutValue(20);
            sheet.Cells["B4"].PutValue(30);

            // Добавить диаграмму в лист
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = sheet.Charts[chartIndex];
            
            // Установить диапазон данных диаграммы
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Получите доступ к области диаграммы
            ChartArea chartArea = chart.ChartArea;
            
            // Продемонстрировать функциональность свойства Area
            Area area = chartArea.Area;
            Console.WriteLine("Original Formatting: " + area.Formatting);
            
            // Изменить свойства области
            area.Formatting = FormattingType.Custom;
            area.BackgroundColor = Color.LightBlue;
            area.ForegroundColor = Color.DarkBlue;
            area.Transparency = 0.3;
            area.InvertIfNegative = true;

            // Сохраните книгу
            workbook.Save("ChartFramePropertyAreaDemo.xlsx");
        }
    }
}
```

### См. также

* class [Area](../../../aspose.cells.drawing/area/)
* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


