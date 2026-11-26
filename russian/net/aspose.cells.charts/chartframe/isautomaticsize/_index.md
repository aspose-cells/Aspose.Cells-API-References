---
title: "ChartFrame.IsAutomaticSize"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ChartFrame. Указывает, автоматически ли задается размер рамки диаграммы"
type: docs
url: /ru/net/aspose.cells.charts/chartframe/isautomaticsize/
---
## ChartFrame.IsAutomaticSize property

Указывает, автоматически ли задаются размеры кадра диаграммы.

```csharp
public virtual bool IsAutomaticSize { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartFramePropertyIsAutomaticSizeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
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
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Установите источник данных диаграммы
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Получить доступ к легенде и продемонстрировать свойство IsAutomaticSize
            Aspose.Cells.Charts.Legend legend = chart.Legend;
            
            // Установить автоматический размер в false и показать значение
            legend.IsAutomaticSize = false;
            Console.WriteLine("Legend Automatic Size: " + legend.IsAutomaticSize);
            
            // Установить автоматический размер в true и показать значение
            legend.IsAutomaticSize = true;
            Console.WriteLine("Legend Automatic Size: " + legend.IsAutomaticSize);
        }
    }
}
```

### См. также

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


