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

    public class CellsUnitTypeDemo
    {
        public static void CellsUnitTypeExample()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Set the default column width in different units
            worksheet.Cells.StandardWidth = 15; // Default unit is characters
            worksheet.Cells.StandardWidthInch = 1.5; // Set width in inches
            worksheet.Cells.StandardWidthPixels = 100; // Set width in pixels

            // Set the default row height in different units
            worksheet.Cells.StandardHeight = 20; // Default unit is points
            worksheet.Cells.StandardHeightInch = 0.5; // Set height in inches
            worksheet.Cells.StandardHeightPixels = 50; // Set height in pixels

            // Set specific column width using CellsUnitType
            worksheet.Cells.SetColumnWidth(0, 20); // Default unit is characters
            worksheet.Cells.SetColumnWidthInch(1, 1.0); // Set width in inches
            worksheet.Cells.SetColumnWidthPixel(2, 80); // Set width in pixels

            // Set specific row height using CellsUnitType
            worksheet.Cells.SetRowHeight(0, 25); // Default unit is points
            worksheet.Cells.SetRowHeightInch(1, 0.4); // Set height in inches
            worksheet.Cells.SetRowHeightPixel(2, 60); // Set height in pixels

            // Save the workbook
            workbook.Save("CellsUnitTypeExample.xlsx");
            workbook.Save("CellsUnitTypeExample.pdf");

            return;
        }
    }
}
```

### See Also

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


