---
title: "ChartCollection.RemoveAt"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод ChartCollection. Удалить диаграмму по конкретному индексу"
type: docs
url: /ru/net/aspose.cells.charts/chartcollection/removeat/
---
## ChartCollection.RemoveAt method

Удалить диаграмму по конкретному индексу.

```csharp
public void RemoveAt(int index)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| индекс | Int32 | Индекс диаграммы. |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartCollectionMethodRemoveAtWithInt32Demo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Добавьте примерные данные для диаграммы
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["B3"].PutValue(20);

            // Добавить диаграмму в лист
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = sheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            // Отобразить начальное количество диаграмм
            Console.WriteLine("Initial chart count: " + sheet.Charts.Count);

            // Удалить диаграмму с индексом 0
            sheet.Charts.RemoveAt(0);

            // Отобразить количество диаграмм после удаления
            Console.WriteLine("Chart count after removal: " + sheet.Charts.Count);
        }
    }
}
```

### См. также

* class [ChartCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


