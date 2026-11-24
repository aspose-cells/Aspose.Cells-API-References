---
title: "Worksheet.ActiveCell"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Worksheet property. Gibt die aktive Zelle zurück oder legt sie fest."
type: docs
url: /de/net/aspose.cells/worksheet/activecell/
---
## Worksheet.ActiveCell property

Liest oder setzt die aktive Zelle im Arbeitsblatt.

```csharp
public string ActiveCell { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyActiveCellDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Setze die aktive Zelle auf B2.
            worksheet.ActiveCell = "B2";
            
            // Gib die Adresse der aktiven Zelle aus.
            Console.WriteLine("Active Cell: " + worksheet.ActiveCell);
            
            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");
            
            // Lade die gespeicherte Arbeitsmappe, um die aktive Zelle zu überprüfen.
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            Console.WriteLine("Loaded Active Cell: " + loadedWorkbook.Worksheets[0].ActiveCell);
        }
    }
}
```

### Siehe auch

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


