---
title: "TimelineCollection.Item"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà TimelineCollection. Ottiene la Timeline per indice"
type: docs
url: /it/net/aspose.cells.timelines/timelinecollection/item/
---
## TimelineCollection indexer (1 of 2)

Ottiene la Timeline per indice.

```csharp
public Timeline this[int index] { get; }
```

### Esempi

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
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet sheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio per la tabella pivot
            sheet.Cells["A1"].PutValue("Date");
            sheet.Cells["A2"].PutValue(DateTime.Now);
            sheet.Cells["A3"].PutValue(DateTime.Now.AddDays(1));
            
            // Crea prima la tabella pivot
            int pivotIndex = sheet.PivotTables.Add("A1:A3", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];
            
            // Aggiungi timeline al foglio di lavoro
            int index = sheet.Timelines.Add(pivotTable, 0, 0, "Date");
            
            // Accedi alla timeline usando la proprietà Item per indice
            Timeline timelineByIndex = sheet.Timelines[index];
            
            // Dimostra l'uso della timeline
            Console.WriteLine("Timeline name: " + timelineByIndex.Name);
        }
    }
}
```

### Vedi anche

* class [Timeline](../../timeline/)
* class [TimelineCollection](../)
* namespace [Aspose.Cells.Timelines](../../../aspose.cells.timelines/)
* assembly [Aspose.Cells](../../../)

---

## TimelineCollection indexer (2 of 2)

Ottiene la Timeline per nome della Timeline.

```csharp
public Timeline this[string name] { get; }
```

### Esempi

```csharp

[C#]

//Ottieni la Timeline per nome della Timeline.
Timeline objByName = sheet.Timelines["date"];
```

### Vedi anche

* class [Timeline](../../timeline/)
* class [TimelineCollection](../)
* namespace [Aspose.Cells.Timelines](../../../aspose.cells.timelines/)
* assembly [Aspose.Cells](../../../)


