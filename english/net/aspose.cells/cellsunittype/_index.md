---
title: Enum CellsUnitType
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.CellsUnitType enum. Specifies the unit of measurement
type: docs
url: /net/aspose.cells/cellsunittype/
---
## CellsUnitType enumeration

Specifies the unit of measurement.

```csharp
public enum CellsUnitType
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| Pixel | `1` | Measurement is in pixels. |
| Point | `2` | Measurement is in points. A point represents 1/72 of an inch. |
| Inch | `4` | Measurement is in inches. |
| Cm | `6` | Measurement is in centimeters. |
| Character | `7` | In unit of characters. |

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsClassCellsUnitTypeDemo
    {
        public static void Run()
        {
            // Create a new workbook for demonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Demonstrate using different CellsUnitType enum values
                Console.WriteLine("Available CellsUnitType values:");

                // Display all enum values
                Console.WriteLine("Pixel: " + CellsUnitType.Pixel);
                Console.WriteLine("Point: " + CellsUnitType.Point);
                Console.WriteLine("Inch: " + CellsUnitType.Inch);
                Console.WriteLine("Cm: " + CellsUnitType.Cm);
                Console.WriteLine("Character: " + CellsUnitType.Character);

                // Example usage: Set column width using different units
                worksheet.Cells.SetColumnWidthPixel(0, 100); // Using Pixel unit
                worksheet.Cells.SetColumnWidthInch(1, 2.0);  // Using Inch unit

                // Save the workbook to demonstrate a complete flow
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

### See Also

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


