---
title: "CellsHelper.DPI"
second_title: "Aspose.Cells för .NET API‑referens"
description: "CellsHelper-egenskap. Hämtar maskinens DPI"
type: docs
url: /sv/net/aspose.cells/cellshelper/dpi/
---
## CellsHelper.DPI property

Hämtar DPI för maskinen.

```csharp
public static double DPI { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsHelperPropertyDPIDemo
    {
        public static void Run()
        {
            // Ange och visa aktuell DPI
            Console.WriteLine("Original DPI: " + CellsHelper.DPI);
            
            // Ändra DPI-inställning
            CellsHelper.DPI = 300;
            Console.WriteLine("New DPI: " + CellsHelper.DPI);

            // Skapa en ny arbetsbok och spara med olika DPI-inställningar
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Lägg till ett exempel på form för att demonstrera DPI-effekten
            sheet.Shapes.AddRectangle(1, 1, 10, 10, 100, 100);

            // Spara med aktuell DPI-inställning
            workbook.Save("output_with_dpi_300.xlsx");

            // Ändra DPI och spara igen
            CellsHelper.DPI = 96;
            workbook.Save("output_with_dpi_96.xlsx");
        }
    }
}
```

### Se även

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


