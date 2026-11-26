---
title: "Timeline.Name"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Timeline. Возвращает или задает имя указанной временной шкалы"
type: docs
url: /ru/net/aspose.cells.timelines/timeline/name/
---
## Timeline.Name property

Возвращает или задаёт имя указанного Timeline

```csharp
public string Name { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class TimelinePropertyNameDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet sheet = workbook.Worksheets[0];
            
            // Добавить примерные данные для временной шкалы
            sheet.Cells["A1"].PutValue("Date");
            sheet.Cells["A2"].PutValue(DateTime.Now.AddDays(-1));
            sheet.Cells["A3"].PutValue(DateTime.Now);
            sheet.Cells["A4"].PutValue(DateTime.Now.AddDays(1));
            
            // Добавить сводную таблицу, которая будет использоваться в качестве источника данных для временной шкалы
            sheet.Cells["C1"].PutValue("Pivot Table");
            int pivotIndex = sheet.PivotTables.Add("A1:A4", "C3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];
            
            // Добавить временную шкалу, используя сводную таблицу
            int timelineIndex = sheet.Timelines.Add(pivotTable, 0, 0, "Timeline1");
            Aspose.Cells.Timelines.Timeline timeline = sheet.Timelines[timelineIndex];
            
            // Установить и продемонстрировать свойство Name
            timeline.Name = "MyTimeline";
            Console.WriteLine("Timeline name: " + timeline.Name);
        }
    }
}
```

### См. также

* class [Timeline](../)
* namespace [Aspose.Cells.Timelines](../../../aspose.cells.timelines/)
* assembly [Aspose.Cells](../../../)


