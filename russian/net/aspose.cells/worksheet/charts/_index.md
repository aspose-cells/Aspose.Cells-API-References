---
title: "Worksheet.Charts"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Worksheet. Возвращает коллекцию Chart"
type: docs
url: /ru/net/aspose.cells/worksheet/charts/
---
## Worksheet.Charts property

Возвращает коллекцию [`Chart`](../../../aspose.cells.charts/chart/) 

```csharp
public ChartCollection Charts { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyChartsDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet sheet = workbook.Worksheets[0];
            
            // Добавить примерные данные для диаграммы
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
            
            // Установите источник данных диаграммы
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // Получите первую серию и задайте шаблон заливки
            Series series = chart.NSeries[0];
            series.Area.FillFormat.Pattern = FillPattern.Solid;
            
            // Сохраните книгу
            workbook.Save("WorksheetPropertyChartsDemo_out.xlsx");
        }
    }
}
```

### См. также

* class [ChartCollection](../../../aspose.cells.charts/chartcollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


