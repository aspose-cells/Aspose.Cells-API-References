---
title: "RangeCollection.Add"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "RangeCollection-Methode. Fügt ein Range-Element zur Sammlung hinzu"
type: docs
url: /de/net/aspose.cells/rangecollection/add/
---
## RangeCollection.Add method

Fügt ein [`Range`](../../range/) Element zur Sammlung hinzu.

```csharp
[Obsolete("Use RangeCollection.AddRange(Range) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Add(Range range)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Bereich | Range | Range-Objekt |

### Hinweise

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die AddRange()-Methode. Diese Methode wird 6 Monate später seit Dezember 2025 entfernt werden. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeCollectionMethodAddWithRangeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Erstellen Sie einen Range und fügen Sie ihn zur Sammlung hinzu
            Aspose.Cells.Range cellRange = worksheet.Cells.CreateRange(0, 0, 3, 1);
            worksheet.Cells.Ranges.Add(cellRange);
            
            // Zeilen einfügen, um zu demonstrieren, dass der Range erweitert wird
            worksheet.Cells.InsertRows(2, 2);
            
            Console.WriteLine("Range row count after insertion: " + cellRange.RowCount);
        }
    }
}
```

### Siehe auch

* class [Range](../../range/)
* class [RangeCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


