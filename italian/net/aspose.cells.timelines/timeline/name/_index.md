---
title: "Timeline.Name"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Timeline. Restituisce o imposta il nome della Timeline specificata"
type: docs
url: /it/net/aspose.cells.timelines/timeline/name/
---
## Timeline.Name property

Restituisce o imposta il nome della Timeline specificata

```csharp
public string Name { get; set; }
```

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet sheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio per la timeline
            sheet.Cells["A1"].PutValue("Date");
            sheet.Cells["A2"].PutValue(DateTime.Now.AddDays(-1));
            sheet.Cells["A3"].PutValue(DateTime.Now);
            sheet.Cells["A4"].PutValue(DateTime.Now.AddDays(1));
            
            // Aggiungi una tabella pivot che verrà usata come origine dati per la timeline
            sheet.Cells["C1"].PutValue("Pivot Table");
            int pivotIndex = sheet.PivotTables.Add("A1:A4", "C3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];
            
            // Aggiungi una timeline usando la tabella pivot
            int timelineIndex = sheet.Timelines.Add(pivotTable, 0, 0, "Timeline1");
            Aspose.Cells.Timelines.Timeline timeline = sheet.Timelines[timelineIndex];
            
            // Imposta e dimostra la proprietà Name
            timeline.Name = "MyTimeline";
            Console.WriteLine("Timeline name: " + timeline.Name);
        }
    }
}
```

### Vedi anche

* class [Timeline](../)
* namespace [Aspose.Cells.Timelines](../../../aspose.cells.timelines/)
* assembly [Aspose.Cells](../../../)


