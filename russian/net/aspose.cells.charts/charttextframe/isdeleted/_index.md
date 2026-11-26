---
title: "ChartTextFrame.IsDeleted"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ChartTextFrame. Указывает, удалена ли эта метка данных"
type: docs
url: /ru/net/aspose.cells.charts/charttextframe/isdeleted/
---
## ChartTextFrame.IsDeleted property

Указывает, удалена ли эта подпись данных.

```csharp
public bool IsDeleted { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartTextFramePropertyIsDeletedDemo
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
            
            // Установите источник данных диаграммы
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Получить доступ к меткам данных и продемонстрировать свойство IsDeleted
            chart.NSeries[0].DataLabels.ShowValue = true;
            bool isDeletedBefore = chart.NSeries[0].DataLabels.IsDeleted;
            
            // Удалить метки данных, установив ShowValue в false
            chart.NSeries[0].DataLabels.ShowValue = false;
            bool isDeletedAfter = chart.NSeries[0].DataLabels.IsDeleted;

            Console.WriteLine($"DataLabels IsDeleted before removal: {isDeletedBefore}");
            Console.WriteLine($"DataLabels IsDeleted after removal: {isDeletedAfter}");
        }
    }
}
```

### См. также

* class [ChartTextFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


