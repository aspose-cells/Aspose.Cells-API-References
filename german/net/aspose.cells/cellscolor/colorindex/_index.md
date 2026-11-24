---
title: "CellsColor.ColorIndex"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "CellsColor-Eigenschaft. Liest und setzt den Farbindex in der Farbpalette. Gilt nur für indizierte Farben"
type: docs
url: /de/net/aspose.cells/cellscolor/colorindex/
---
## CellsColor.ColorIndex property

Liest und setzt den Farbindex in der Farbpalette. Gilt nur für indizierte Farben.

```csharp
public int ColorIndex { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using System;
    using Aspose.Cells;

    public class CellsColorPropertyColorIndexDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine neue Arbeitsmappe und rufen Sie das erste Arbeitsblatt ab
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Definieren Sie einen Bereich, auf den wir einen farbigen Rahmen anwenden werden
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("B2:D4");

            // Erstellen Sie eine CellsColor‑Instanz
            CellsColor cellsColor = workbook.CreateCellsColor();

            // Setzen Sie den ColorIndex (Palettenindex) – zum Beispiel 5
            cellsColor.ColorIndex = 5;

            // Wenden Sie das CellsColor als Innenrahmenfarbe des Bereichs an
            range.SetInsideBorders(BorderType.Horizontal | BorderType.Vertical,
                                   CellBorderType.Thin,
                                   cellsColor);

            // Lesen und anzeigen Sie den aktuellen ColorIndex-Wert
            Console.WriteLine("Current ColorIndex value: " + cellsColor.ColorIndex);

            // Speichere die Arbeitsmappe, um das Ergebnis zu visualisieren
            try
            {
                workbook.Save("ColorIndexDemo.xlsx");
                Console.WriteLine("Workbook saved as ColorIndexDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error saving workbook: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* class [CellsColor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


