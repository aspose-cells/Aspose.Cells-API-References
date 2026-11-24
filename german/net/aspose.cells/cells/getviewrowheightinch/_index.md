---
title: "Cells.GetViewRowHeightInch"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cells-Methode. Gibt die Höhe einer angegebenen Zeile in der Einheit Zoll zurück"
type: docs
url: /de/net/aspose.cells/cells/getviewrowheightinch/
---
## Cells.GetViewRowHeightInch method

Gibt die Höhe einer angegebenen Zeile in Zoll zurück.

```csharp
public double GetViewRowHeightInch(int row)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| row | Int32 | Zeilenindex |

### Rückgabewert

Höhe der Zeile

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodGetViewRowHeightInchWithInt32Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Benutzerdefinierte Zeilenhöhe für Zeile 2 in Zoll festlegen
            worksheet.Cells.SetRowHeightInch(2, 1.5);

            try
            {
                // Rufen Sie GetViewRowHeightInch mit dem Zeilenindex-Parameter auf
                double rowHeight = worksheet.Cells.GetViewRowHeightInch(2);
                
                // Ergebnis anzeigen und prüfen, ob die Höhe dem festgelegten Wert entspricht
                Console.WriteLine($"View row height of row 2: {rowHeight} inches");
                
                // Demonstriere die Wirkung, indem du Beispielinhalt hinzufügst
                worksheet.Cells["A2"].PutValue($"Row Height: {rowHeight}\"");
                worksheet.Cells.SetColumnWidthInch(0, 15);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetViewRowHeightInch: {ex.Message}");
            }
            
            // Speichere die geänderte Arbeitsmappe
            workbook.Save("CellsMethodGetViewRowHeightInchWithInt32Demo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


