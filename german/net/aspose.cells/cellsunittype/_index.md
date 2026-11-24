---
title: "Enum CellsUnitType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.CellsUnitType Enum. Gibt die Maßeinheit an"
type: docs
url: /de/net/aspose.cells/cellsunittype/
---
## CellsUnitType enumeration

Gibt die Maßeinheit an.

```csharp
public enum CellsUnitType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| Pixel | `1` | Messung erfolgt in Pixeln. |
| Point | `2` | Messung erfolgt in Punkten. Ein Punkt entspricht 1/72 Zoll. |
| Inch | `4` | Messung erfolgt in Zoll. |
| Cm | `6` | Messung erfolgt in Zentimetern. |
| Character | `7` | In Einheiten von Zeichen. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsClassCellsUnitTypeDemo
    {
        public static void Run()
        {
            // Erstellt ein neues Arbeitsbuch für die Demonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Demonstriere die Verwendung verschiedener CellsUnitType-Enum-Werte
                Console.WriteLine("Available CellsUnitType values:");

                // Alle Enum-Werte anzeigen
                Console.WriteLine("Pixel: " + CellsUnitType.Pixel);
                Console.WriteLine("Point: " + CellsUnitType.Point);
                Console.WriteLine("Inch: " + CellsUnitType.Inch);
                Console.WriteLine("Cm: " + CellsUnitType.Cm);
                Console.WriteLine("Character: " + CellsUnitType.Character);

                // Beispielhafte Verwendung: Spaltenbreite mit verschiedenen Einheiten festlegen
                worksheet.Cells.SetColumnWidthPixel(0, 100); // Using Pixel unit
                worksheet.Cells.SetColumnWidthInch(1, 2.0);  // Using Inch unit

                // Speichere die Arbeitsmappe, um einen vollständigen Ablauf zu demonstrieren
                workbook.Save("CellsUnitTypeDemo.xlsx");
                Console.WriteLine("Workbook saved successfully with different unit types applied.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with CellsUnitType: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


