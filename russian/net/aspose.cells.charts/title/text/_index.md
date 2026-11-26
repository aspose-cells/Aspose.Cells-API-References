---
title: "Title.Text"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Title. Возвращает или задает текст метки единицы отображения"
type: docs
url: /ru/net/aspose.cells.charts/title/text/
---
## Title.Text property

Получает или задает текст метки единицы отображения.

```csharp
public override string Text { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class TitlePropertyTextDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получите доступ к первому листу и добавьте примерные данные
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Q1");
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(200);
            worksheet.Cells["A4"].PutValue(300);
            
            // Добавить диаграмму и задать текст заголовка ValueAxis
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.ValueAxis.Title.Text = "Sales Amount";
            
            // Сохраните книгу
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [Title](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


