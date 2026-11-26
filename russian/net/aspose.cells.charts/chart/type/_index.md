---
title: "Chart.Type"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Chart. Возвращает или задаёт тип диаграммы"
type: docs
url: /ru/net/aspose.cells.charts/chart/type/
---
## Chart.Type property

Получает или задает тип диаграммы.

```csharp
public ChartType Type { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyTypeDemo
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

            // Добавьте радиальную диаграмму
            int chartIndex = sheet.Charts.Add(ChartType.Radar, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = sheet.Charts[chartIndex];
            
            // Установить диапазон данных диаграммы
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Продемонстрировать использование свойства Type
            Console.WriteLine("Chart type is: " + chart.Type);
            
            // Измените тип диаграммы на столбчатый
            chart.Type = ChartType.Column;
            Console.WriteLine("Chart type changed to: " + chart.Type);
        }
    }
}
```

### См. также

* enum [ChartType](../../charttype/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


