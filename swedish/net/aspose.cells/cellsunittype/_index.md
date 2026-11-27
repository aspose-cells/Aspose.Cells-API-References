---
title: "Enum CellsUnitType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.CellsUnitType‑enum. Anger måttenheten"
type: docs
url: /sv/net/aspose.cells/cellsunittype/
---
## CellsUnitType enumeration

Anger mätenheten.

```csharp
public enum CellsUnitType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Pixel | `1` | Mätning är i pixlar. |
| Point | `2` | Mätning är i punkter. En punkt motsvarar 1/72 tum. |
| Inch | `4` | Mätning är i tum. |
| Cm | `6` | Mätning är i centimeter. |
| Character | `7` | I teckenenhet. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsClassCellsUnitTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok för demonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Demonstrera användning av olika CellsUnitType‑enum‑värden
                Console.WriteLine("Available CellsUnitType values:");

                // Visa alla enum‑värden
                Console.WriteLine("Pixel: " + CellsUnitType.Pixel);
                Console.WriteLine("Point: " + CellsUnitType.Point);
                Console.WriteLine("Inch: " + CellsUnitType.Inch);
                Console.WriteLine("Cm: " + CellsUnitType.Cm);
                Console.WriteLine("Character: " + CellsUnitType.Character);

                // Exempel på användning: Ställ in kolumnbredd med olika enheter
                worksheet.Cells.SetColumnWidthPixel(0, 100); // Using Pixel unit
                worksheet.Cells.SetColumnWidthInch(1, 2.0);  // Using Inch unit

                // Spara arbetsboken för att demonstrera ett komplett flöde
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

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


