---
title: "WorksheetCollection.GetNamedRangesAndTables"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WorksheetCollection-Methode. Ruft alle vordefinierten benannten Bereiche im Tabellenblatt ab"
type: docs
url: /de/net/aspose.cells/worksheetcollection/getnamedrangesandtables/
---
## WorksheetCollection.GetNamedRangesAndTables method

Ruft alle vordefinierten benannten Bereiche im Tabellenblatt ab.

```csharp
public Range[] GetNamedRangesAndTables()
```

### Rückgabewert

Ein Array von Range-Objekten.

Gibt null zurück, wenn der benannte Bereich nicht existiert.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodGetNamedRangesAndTablesDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Erstelle einige benannte Bereiche
            worksheet.Cells.CreateRange("A1:B2").Name = "TestRange1";
            worksheet.Cells.CreateRange("C3:D4").Name = "TestRange2";
            
            // Rufe alle benannten Bereiche und Tabellen ab
            Aspose.Cells.Range[] ranges = workbook.Worksheets.GetNamedRangesAndTables();
            
            // Zeige Informationen zu den Bereichen an
            Console.WriteLine("Found {0} named ranges:", ranges.Length);
            foreach (Aspose.Cells.Range range in ranges)
            {
                Console.WriteLine("Name: {0}, Address: {1}", range.Name, range.Address);
            }
        }
    }
}
```

### Siehe auch

* class [Range](../../range/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


