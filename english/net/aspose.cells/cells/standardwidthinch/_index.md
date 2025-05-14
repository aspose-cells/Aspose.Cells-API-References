---
title: Cells.StandardWidthInch
second_title: Aspose.Cells for .NET API Reference
description: Cells property. Gets or sets the default column width in the worksheet in unit of inches
type: docs
url: /net/aspose.cells/cells/standardwidthinch/
---
## Cells.StandardWidthInch property

Gets or sets the default column width in the worksheet, in unit of inches.

```csharp
public double StandardWidthInch { get; set; }
```

### Examples

```csharp
// Called: worksheet.Cells.StandardWidthInch = 1.5; // Set width in inches
public static void Cells_Property_StandardWidthInch()
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
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


