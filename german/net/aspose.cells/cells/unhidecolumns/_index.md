---
title: "Cells.UnhideColumns"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cells‑Methode. Blendet mehrere Spalten ein."
type: docs
url: /de/net/aspose.cells/cells/unhidecolumns/
---
## Cells.UnhideColumns method

Blendet mehrere Spalten ein.

```csharp
public void UnhideColumns(int column, int totalColumns, double width)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| column | Int32 | Spaltenindex. |
| totalColumns | Int32 | Spaltennummer |
| Breite | Double | Spaltenbreite. |

### Hinweise

Wendet die Spaltenbreite nur auf die ausgeblendeten Spalten an.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodUnhideColumnsWithInt32Int32DoubleDemo
    {
        public static void Run()
        {
            // Erstelle eine neue Arbeitsmappe und greife auf das erste Arbeitsblatt zu
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Spalten 1-3 (nullbasiert) zunächst ausblenden
            worksheet.Cells.HideColumns(1, 3);

            try
            {
                // Spalten ab Index 1 (zweite Spalte) wieder einblenden, 3 Spalten breit, Breite auf 15.5 setzen
                worksheet.Cells.UnhideColumns(1, 3, 15.5);

                // Überprüfen Sie die wieder eingeblendeten Spalten, indem Sie deren Breite prüfen
                Console.WriteLine($"Column 1 width after unhiding: {worksheet.Cells.GetColumnWidth(1)}");
                Console.WriteLine("Columns 1-3 successfully unhidden with specified width");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing UnhideColumns: {ex.Message}");
            }

            // Speichere die geänderte Arbeitsmappe
            workbook.Save("UnhideColumnsWithWidthDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


