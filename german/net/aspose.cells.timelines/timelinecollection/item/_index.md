---
title: "TimelineCollection.Item"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "TimelineCollection-Eigenschaft. Gibt die Zeitachse anhand des Index zurück"
type: docs
url: /de/net/aspose.cells.timelines/timelinecollection/item/
---
## TimelineCollection indexer (1 of 2)

Gibt die Zeitachse anhand des Index zurück.

```csharp
public Timeline this[int index] { get; }
```

### Beispiele

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
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet sheet = workbook.Worksheets[0];
            
            // Füge Beispieldaten für die Pivot‑Tabelle hinzu
            sheet.Cells["A1"].PutValue("Date");
            sheet.Cells["A2"].PutValue(DateTime.Now);
            sheet.Cells["A3"].PutValue(DateTime.Now.AddDays(1));
            
            // Zuerst Pivot-Tabelle erstellen
            int pivotIndex = sheet.PivotTables.Add("A1:A3", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];
            
            // Zeitachse zum Arbeitsblatt hinzufügen
            int index = sheet.Timelines.Add(pivotTable, 0, 0, "Date");
            
            // Zugriff auf die Zeitachse mittels Item-Eigenschaft nach Index
            Timeline timelineByIndex = sheet.Timelines[index];
            
            // Verwendung der Zeitachse demonstrieren
            Console.WriteLine("Timeline name: " + timelineByIndex.Name);
        }
    }
}
```

### Siehe auch

* class [Timeline](../../timeline/)
* class [TimelineCollection](../)
* namespace [Aspose.Cells.Timelines](../../../aspose.cells.timelines/)
* assembly [Aspose.Cells](../../../)

---

## TimelineCollection indexer (2 of 2)

Gibt die Zeitachse anhand ihres Namens zurück.

```csharp
public Timeline this[string name] { get; }
```

### Beispiele

```csharp

[C#]

//Hole die Zeitachse anhand ihres Namens.
Timeline objByName = sheet.Timelines["date"];
```

### Siehe auch

* class [Timeline](../../timeline/)
* class [TimelineCollection](../)
* namespace [Aspose.Cells.Timelines](../../../aspose.cells.timelines/)
* assembly [Aspose.Cells](../../../)


