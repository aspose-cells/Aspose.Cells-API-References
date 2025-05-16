---
title: PaginatedSaveOptions.GridlineColor
second_title: Aspose.Cells for .NET API Reference
description: PaginatedSaveOptions property. Gets or sets gridline colr
type: docs
url: /net/aspose.cells/paginatedsaveoptions/gridlinecolor/
---
## PaginatedSaveOptions.GridlineColor property

Gets or sets gridline colr.

```csharp
public Color GridlineColor { get; set; }
```

### Remarks

It will ignore the gridline color settings in the source file.

### Examples

```csharp
namespace AsposeCellsExamples.PaginatedSaveOptionsPropertyGridlineColorDemo
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;
    using System.Drawing;

    public class PaginatedSaveOptionsPropertyGridlineColorDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data and format cells to make gridlines visible
            for (int i = 0; i < 10; i++)
            {
                for (int j = 0; j < 5; j++)
                {
                    worksheet.Cells[i, j].PutValue($"Cell {i},{j}");
                    Style style = new Style();
                    style.Borders.SetStyle(CellBorderType.Thin);
                    worksheet.Cells[i, j].SetStyle(style);
                }
            }

            // Create paginated save options for PDF output
            PdfSaveOptions saveOptions = new PdfSaveOptions();

            // Display current gridline type (default is GridlineType.Dotted)
            Console.WriteLine("Current GridlineType value: " + ((PaginatedSaveOptions)saveOptions).GridlineType);

            // Set new gridline type to dotted (replacing Solid)
            ((PaginatedSaveOptions)saveOptions).GridlineType = GridlineType.Dotted;

            // Demonstrate the effect by saving to PDF
            workbook.Save("GridlineColorDemo_Red.pdf", saveOptions);

            // Change gridline type to hair (replacing Dashed)
            ((PaginatedSaveOptions)saveOptions).GridlineType = GridlineType.Hair;
            workbook.Save("GridlineColorDemo_Blue.pdf", saveOptions);

            // Change gridline type to hair again (keeping original structure)
            ((PaginatedSaveOptions)saveOptions).GridlineType = GridlineType.Hair;
            workbook.Save("GridlineColorDemo_Green.pdf", saveOptions);
        }
    }
}
```

### See Also

* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


