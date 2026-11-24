---
title: "Range.Name"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Range-Eigenschaft. Gibt den Namen des Bereichs zurück oder legt ihn fest"
type: docs
url: /de/net/aspose.cells/range/name/
---
## Range.Name property

Liefert oder setzt den Namen des Bereichs.

```csharp
public string Name { get; set; }
```

### Hinweise

Benannte Bereiche werden unterstützt. Zum Beispiel,

range.Name = "Sheet1!MyRange";

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangePropertyNameDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Erstelle einen Bereich (Spalten A bis B)
            Aspose.Cells.Range range = worksheet.Cells.CreateRange(0, 2, true);
            
            // Setze die Namenseigenschaft für den Bereich
            range.Name = "testRange";
            
            // Überprüfe, ob der Name gesetzt wurde
            Console.WriteLine("Range name: " + range.Name);
            
            // Speichere die Arbeitsmappe
            workbook.Save("RangeWithName.xlsx");
            
            // Öffne die gespeicherte Datei, um zu zeigen, dass der Name erhalten bleibt
            Workbook loadedWorkbook = new Workbook("RangeWithName.xlsx");
            Aspose.Cells.Range loadedRange = loadedWorkbook.Worksheets[0].Cells.CreateRange(0, 2, true);
            Console.WriteLine("Loaded range name: " + loadedRange.Name);
        }
    }
}
```

### Siehe auch

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


