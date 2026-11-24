---
title: "Cells.GetColumnOriginalWidthPoint"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cells-Methode. Gibt die ursprüngliche Spaltenhöhe in Punkt zurück, wenn die Spalte ausgeblendet ist."
type: docs
url: /de/net/aspose.cells/cells/getcolumnoriginalwidthpoint/
---
## Cells.GetColumnOriginalWidthPoint method

Gibt die ursprüngliche Spaltenhöhe in Punkt zurück, wenn die Spalte ausgeblendet ist.

```csharp
[Obsolete("Use Cells.GetColumnWidth(int ,bool , CellsUnitType ) method, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public double GetColumnOriginalWidthPoint(int column)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| column | Int32 | Der Zeilenindex. |

### Rückgabewert

Breite der Spalte in der Normalansicht.

### Hinweise

HINWEIS: Diese Methode ist jetzt veraltet. Bitte verwenden Sie stattdessen die Methode Cells.GetColumnWidth(int ,bool , CellsUnitType ). Diese Methode wird 12 Monate nach April 2024 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Ihnen entstanden sein könnten.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodGetColumnOriginalWidthPointWithInt32Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Spaltenindex-Parameter vorbereiten.
            int columnIndex = 0;

            try
            {
                // Ursprüngliche Spaltenbreite in Punkten abrufen.
                double originalWidth = cells.GetColumnOriginalWidthPoint(columnIndex);
                Console.WriteLine($"Original width of column {columnIndex}: {originalWidth} points");

                // Spaltenbreite ändern.
                cells.SetColumnWidth(columnIndex, 15);
                Console.WriteLine("Set new column width to 15 points");

                // Ursprüngliche Breite erneut abrufen, um zu zeigen, dass sie unverändert bleibt.
                double unchangedWidth = cells.GetColumnOriginalWidthPoint(columnIndex);
                Console.WriteLine($"Original width remains: {unchangedWidth} points");

                // Aktuelle Breite abrufen, um die Änderung zu zeigen.
                double currentWidth = cells.GetColumnWidth(columnIndex);
                Console.WriteLine($"Current column width: {currentWidth} points");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetColumnOriginalWidthPoint method: {ex.Message}");
            }

            // Speichere die geänderte Arbeitsmappe
            workbook.Save("GetColumnOriginalWidthPointDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


