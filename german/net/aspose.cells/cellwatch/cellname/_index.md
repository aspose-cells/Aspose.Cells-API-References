---
title: "CellWatch.CellName"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "CellWatch-Eigenschaft. Liest und schreibt den Namen der Zelle."
type: docs
url: /de/net/aspose.cells/cellwatch/cellname/
---
## CellWatch.CellName property

Ermittelt und setzt den Namen der Zelle.

```csharp
public string CellName { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellWatchPropertyCellNameDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Füge einige CellWatch-Instanzen hinzu.
            worksheet.CellWatches.Add("B5");
            worksheet.CellWatches.Add("C10");
            
            // Zeige die Zellnamen aller CellWatch-Instanzen an.
            Console.WriteLine("Cell Watches:");
            foreach (CellWatch watch in worksheet.CellWatches)
            {
                Console.WriteLine(watch.CellName);
            }
            
            // Füge einen neuen CellWatch hinzu und zeige dessen Namen an.
            worksheet.CellWatches.Add("A1");
            Console.WriteLine("Added new watch: " + 
                worksheet.CellWatches[worksheet.CellWatches.Count - 1].CellName);
            
            // Speichere die Arbeitsmappe
            workbook.Save("CellWatchDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [CellWatch](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


