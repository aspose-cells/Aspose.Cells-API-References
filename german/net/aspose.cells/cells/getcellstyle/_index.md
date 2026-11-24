---
title: "Cells.GetCellStyle"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cells-Methode. Gibt den Stil der angegebenen Zelle zurück"
type: docs
url: /de/net/aspose.cells/cells/getcellstyle/
---
## Cells.GetCellStyle method

Ermittelt den Stil der angegebenen Zelle.

```csharp
public Style GetCellStyle(int row, int column)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| row | Int32 | Zeilenindex |
| column | Int32 | column |

### Rückgabewert

der Stil der angegebenen Zelle.

### Hinweise

Der zurückgegebene Stil ist nur der für die Zelle festgelegte oder von der Zeile/Spalte der Zelle vererbte Stil und enthält nicht die durch andere Einstellungen wie bedingte Formatierungen angewendeten Eigenschaften.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class CellsMethodGetCellStyleWithInt32Int32Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Zugriff auf Zelle B5 (Zeile 4, Spalte 1) und initialen Stil festlegen
            Cell cell = worksheet.Cells["B5"];
            cell.PutValue("Styled Cell");
            
            // Initialen Zellenstil erstellen und anwenden
            Style initialStyle = workbook.CreateStyle();
            initialStyle.Font.IsBold = true;  // Changed from Bold to IsBold
            initialStyle.BackgroundColor = Color.LightYellow;
            cell.SetStyle(initialStyle);

            try
            {
                // GetCellStyle mit Int32-Parametern aufrufen (Zeile 4, Spalte 1)
                Style cellStyle = worksheet.Cells.GetCellStyle(4, 1);

                // Abgerufene Stileigenschaften anzeigen
                Console.WriteLine($"Retrieved style - Bold: {cellStyle.Font.IsBold}, Background: {cellStyle.BackgroundColor}");  // Changed from Bold to IsBold

                // Den abgerufenen Stil ändern
                cellStyle.Font.IsItalic = true;  // Changed from Italic to IsItalic
                cellStyle.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thin;

                // Den geänderten Stil wieder auf die Zelle anwenden
                cell.SetStyle(cellStyle);

                Console.WriteLine("GetCellStyle executed successfully. Modified border and font style.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetCellStyle: {ex.Message}");
            }

            // Speichere die geänderte Arbeitsmappe
            workbook.Save("CellsGetCellStyleWithInt32Demo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Style](../../style/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


