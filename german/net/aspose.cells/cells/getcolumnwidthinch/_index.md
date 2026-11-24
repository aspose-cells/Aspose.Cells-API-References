---
title: "Cells.GetColumnWidthInch"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cells-Methode. Gibt die Breite der angegebenen Spalte in der Normalansicht in Zoll zurück"
type: docs
url: /de/net/aspose.cells/cells/getcolumnwidthinch/
---
## Cells.GetColumnWidthInch method

Gibt die Breite der angegebenen Spalte in der Normalansicht in Zoll zurück.

```csharp
[Obsolete("Use Cells.GetColumnWidth(int ,bool , CellsUnitType ) method, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public double GetColumnWidthInch(int column)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| column | Int32 | Spaltenindex |

### Rückgabewert

Spaltenbreite

Breite der Spalte in der Normalansicht.

### Hinweise

HINWEIS: Diese Methode ist jetzt veraltet. Bitte verwenden Sie stattdessen die Methode Cells.GetColumnWidth(int ,bool , CellsUnitType ). Diese Methode wird 12 Monate nach April 2024 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Ihnen entstanden sein könnten.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodGetColumnWidthInchWithInt32Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Spaltenbreite in Zoll für die Demonstration festlegen
            int columnIndex = 2;
            cells.SetColumnWidthInch(columnIndex, 2.5);

            try
            {
                // Rufen Sie GetColumnWidthInch mit dem Int32-Parameter auf
                double columnWidth = cells.GetColumnWidthInch(columnIndex);

                // Ergebnis anzeigen
                Console.WriteLine($"Width of column {columnIndex} in inches: {columnWidth}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetColumnWidthInch method: {ex.Message}");
            }

            // Speichere die Arbeitsmappe
            workbook.Save("CellsMethodGetColumnWidthInchDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


