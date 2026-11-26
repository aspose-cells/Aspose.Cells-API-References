---
title: "TickLabels.NumberFormatLinked"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство TickLabels. Истина, если числовой формат связан с ячейками, так что изменение формата в ячейках приводит к изменению формата в метках"
type: docs
url: /ru/net/aspose.cells.charts/ticklabels/numberformatlinked/
---
## TickLabels.NumberFormatLinked property

True, если числовой формат связан с ячейками (чтобы формат числа менялся в метках, когда он меняется в ячейках).

```csharp
public bool NumberFormatLinked { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class TickLabelsPropertyNumberFormatLinkedDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue(100);
            worksheet.Cells["A2"].PutValue(200);
            worksheet.Cells["A3"].PutValue(300);
            worksheet.Cells["A4"].PutValue(400);
            
            // Добавьте диаграмму
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Установите источник данных диаграммы
            chart.NSeries.Add("A1:A4", true);
            
            // Получить доступ к меткам делений оси значений
            Aspose.Cells.Charts.TickLabels tickLabels = chart.ValueAxis.TickLabels;
            
            // Продемонстрировать свойство NumberFormatLinked
            Console.WriteLine("NumberFormatLinked (default): " + tickLabels.NumberFormatLinked);
            
            // Изменить свойство
            tickLabels.NumberFormatLinked = false;
            Console.WriteLine("NumberFormatLinked after change: " + tickLabels.NumberFormatLinked);
            
            // Сохраните книгу
            workbook.Save("TickLabelsNumberFormatLinkedDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### См. также

* class [TickLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


