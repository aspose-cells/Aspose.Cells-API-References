---
title: "TimelineCollection.Item"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TimelineCollection-egenskap. Hämtar tidslinjen efter index"
type: docs
url: /sv/net/aspose.cells.timelines/timelinecollection/item/
---
## TimelineCollection indexer (1 of 2)

Hämtar tidslinjen efter index.

```csharp
public Timeline this[int index] { get; }
```

### Exempel

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
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet sheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata för pivottabell
            sheet.Cells["A1"].PutValue("Date");
            sheet.Cells["A2"].PutValue(DateTime.Now);
            sheet.Cells["A3"].PutValue(DateTime.Now.AddDays(1));
            
            // Skapa pivottabell först
            int pivotIndex = sheet.PivotTables.Add("A1:A3", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];
            
            // Lägg till tidslinje i kalkylbladet
            int index = sheet.Timelines.Add(pivotTable, 0, 0, "Date");
            
            // Åtkomst till tidslinje med Item-egenskapen efter index
            Timeline timelineByIndex = sheet.Timelines[index];
            
            // Demonstrera användning av tidslinjen
            Console.WriteLine("Timeline name: " + timelineByIndex.Name);
        }
    }
}
```

### Se även

* class [Timeline](../../timeline/)
* class [TimelineCollection](../)
* namespace [Aspose.Cells.Timelines](../../../aspose.cells.timelines/)
* assembly [Aspose.Cells](../../../)

---

## TimelineCollection indexer (2 of 2)

Hämtar tidslinjen efter tidslinjens namn.

```csharp
public Timeline this[string name] { get; }
```

### Exempel

```csharp

[C#]

//Hämta tidslinjen efter tidslinjens namn.
Timeline objByName = sheet.Timelines["date"];
```

### Se även

* class [Timeline](../../timeline/)
* class [TimelineCollection](../)
* namespace [Aspose.Cells.Timelines](../../../aspose.cells.timelines/)
* assembly [Aspose.Cells](../../../)


