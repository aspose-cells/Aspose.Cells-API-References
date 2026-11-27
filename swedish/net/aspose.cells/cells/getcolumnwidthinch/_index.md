---
title: "Cells.GetColumnWidthInch"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cells-metod. Hämtar bredden på den angivna kolumnen i normal vy i tum"
type: docs
url: /sv/net/aspose.cells/cells/getcolumnwidthinch/
---
## Cells.GetColumnWidthInch method

Hämtar bredden på den angivna kolumnen i normal vy, i tum.

```csharp
[Obsolete("Use Cells.GetColumnWidth(int ,bool , CellsUnitType ) method, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public double GetColumnWidthInch(int column)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| column | Int32 | Kolumnindex |

### Returvärde

Kolumnbredd

Kolumnens bredd i normal vy.

### Anmärkningar

OBS: Denna metod är nu föråldrad. Använd istället Cells.GetColumnWidth(int ,bool , CellsUnitType )-metoden. Denna metod kommer att tas bort 12 månader senare från och med april 2024. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodGetColumnWidthInchWithInt32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Ställ in kolumnbredd i tum för demonstration
            int columnIndex = 2;
            cells.SetColumnWidthInch(columnIndex, 2.5);

            try
            {
                // Anropa GetColumnWidthInch med Int32-parameter
                double columnWidth = cells.GetColumnWidthInch(columnIndex);

                // Visa resultatet
                Console.WriteLine($"Width of column {columnIndex} in inches: {columnWidth}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetColumnWidthInch method: {ex.Message}");
            }

            // Spara arbetsboken
            workbook.Save("CellsMethodGetColumnWidthInchDemo.xlsx");
        }
    }
}
```

### Se även

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


