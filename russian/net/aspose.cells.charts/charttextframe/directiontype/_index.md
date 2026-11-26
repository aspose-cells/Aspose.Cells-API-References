---
title: "ChartTextFrame.DirectionType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ChartTextFrame. Получает и задает направление текста"
type: docs
url: /ru/net/aspose.cells.charts/charttextframe/directiontype/
---
## ChartTextFrame.DirectionType property

Получает и задает направление текста.

```csharp
public virtual ChartTextDirectionType DirectionType { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartTextFramePropertyDirectionTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            // Добавление листа возвращает его индекс, затем мы получаем лист по индексу
            int sheetIndex = workbook.Worksheets.Add();
            Worksheet worksheet = workbook.Worksheets[sheetIndex];
            
            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);
            worksheet.Cells["C1"].PutValue("Q1");
            worksheet.Cells["C2"].PutValue("Q2");
            worksheet.Cells["C3"].PutValue("Q3");

            // Добавить диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:B3", true);
            chart.NSeries.CategoryData = "C1:C3";

            // Получить доступ и настроить заголовок
            ChartTextFrame title = chart.Title;
            title.Text = "Sample Chart";
            
            // Продемонстрировать свойство DirectionType
            title.DirectionType = ChartTextDirectionType.Vertical;
            
            // Сохраните книгу
            workbook.Save("ChartTextDirectionDemo.xlsx");
        }
    }
}
```

### См. также

* enum [ChartTextDirectionType](../../charttextdirectiontype/)
* class [ChartTextFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


