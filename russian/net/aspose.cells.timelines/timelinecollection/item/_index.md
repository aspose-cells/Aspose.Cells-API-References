---
title: "TimelineCollection.Item"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство TimelineCollection. Получает Timeline по индексу"
type: docs
url: /ru/net/aspose.cells.timelines/timelinecollection/item/
---
## TimelineCollection indexer (1 of 2)

Получает Timeline по индексу.

```csharp
public Timeline this[int index] { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Timelines;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class TimelineCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet sheet = workbook.Worksheets[0];
            
            // Добавить примерные данные для сводной таблицы
            sheet.Cells["A1"].PutValue("Date");
            sheet.Cells["A2"].PutValue(DateTime.Now);
            sheet.Cells["A3"].PutValue(DateTime.Now.AddDays(1));
            
            // Сначала создайте сводную таблицу
            int pivotIndex = sheet.PivotTables.Add("A1:A3", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];
            
            // Добавить Timeline на лист
            int index = sheet.Timelines.Add(pivotTable, 0, 0, "Date");
            
            // Получить доступ к Timeline, используя свойство Item по индексу
            Timeline timelineByIndex = sheet.Timelines[index];
            
            // Продемонстрировать использование Timeline
            Console.WriteLine("Timeline name: " + timelineByIndex.Name);
        }
    }
}
```

### См. также

* class [Timeline](../../timeline/)
* class [TimelineCollection](../)
* namespace [Aspose.Cells.Timelines](../../../aspose.cells.timelines/)
* assembly [Aspose.Cells](../../../)

---

## TimelineCollection indexer (2 of 2)

Получает Timeline по имени Timeline.

```csharp
public Timeline this[string name] { get; }
```

### Примеры

```csharp

[C#]

//Получить Timeline по имени Timeline.
Timeline objByName = sheet.Timelines["date"];
```

### См. также

* class [Timeline](../../timeline/)
* class [TimelineCollection](../)
* namespace [Aspose.Cells.Timelines](../../../aspose.cells.timelines/)
* assembly [Aspose.Cells](../../../)


