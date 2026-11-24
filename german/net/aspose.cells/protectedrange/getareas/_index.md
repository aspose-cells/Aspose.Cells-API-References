---
title: "ProtectedRange.GetAreas"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ProtectedRange-Methode. Gibt alle referenzierten Bereiche zurück"
type: docs
url: /de/net/aspose.cells/protectedrange/getareas/
---
## ProtectedRange.GetAreas method

Ruft alle referenzierten Bereiche ab.

```csharp
public CellArea[] GetAreas()
```

### Rückgabewert

Gibt alle referenzierten Bereiche zurück.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectedRangeMethodGetAreasDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            
            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Rufe die Sammlung geschützter Bereiche ab
            ProtectedRangeCollection protectedRanges = worksheet.AllowEditRanges;
            
            // Füge einen geschützten Bereich hinzu
            int index = protectedRanges.Add("TestRange", 0, 0, 10, 10);
            ProtectedRange protectedRange = protectedRanges[index];
            
            // Rufe die Bereiche des geschützten Bereichs ab
            CellArea[] areas = protectedRange.GetAreas();
            
            // Gib die Anzahl der Bereiche aus (sollte für diesen einfachen Bereich 1 sein)
            Console.WriteLine("Number of areas in protected range: " + areas.Length);
            
            // Speichere die Arbeitsmappe
            workbook.Save("ProtectedRangeExample.xlsx");
        }
    }
}
```

### Siehe auch

* struct [CellArea](../../cellarea/)
* class [ProtectedRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


