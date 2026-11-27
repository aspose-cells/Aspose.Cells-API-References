---
title: "Cells.GetColumnOriginalWidthPoint"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cells-metoden. Hämtar originalhöjden för kolumner i enheten punkt om kolumnen är dold"
type: docs
url: /sv/net/aspose.cells/cells/getcolumnoriginalwidthpoint/
---
## Cells.GetColumnOriginalWidthPoint method

Hämtar originalhöjden för kolumnen i enheten punkt om kolumnen är dold

```csharp
[Obsolete("Use Cells.GetColumnWidth(int ,bool , CellsUnitType ) method, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public double GetColumnOriginalWidthPoint(int column)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| column | Int32 | Radindexet. |

### Returvärde

Kolumnens bredd i normal vy.

### Anmärkningar

OBS: Denna metod är nu föråldrad. Använd istället Cells.GetColumnWidth(int ,bool , CellsUnitType )-metoden. Denna metod kommer att tas bort 12 månader senare från och med april 2024. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodGetColumnOriginalWidthPointWithInt32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Förbered kolumnindexparameter
            int columnIndex = 0;

            try
            {
                // Hämta originalkolumnbredd i punkter
                double originalWidth = cells.GetColumnOriginalWidthPoint(columnIndex);
                Console.WriteLine($"Original width of column {columnIndex}: {originalWidth} points");

                // Ändra kolumnbredd
                cells.SetColumnWidth(columnIndex, 15);
                Console.WriteLine("Set new column width to 15 points");

                // Hämta originalbredden igen för att visa att den förblir oförändrad
                double unchangedWidth = cells.GetColumnOriginalWidthPoint(columnIndex);
                Console.WriteLine($"Original width remains: {unchangedWidth} points");

                // Hämta aktuell bredd för att visa ändring
                double currentWidth = cells.GetColumnWidth(columnIndex);
                Console.WriteLine($"Current column width: {currentWidth} points");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetColumnOriginalWidthPoint method: {ex.Message}");
            }

            // Spara den modifierade arbetsboken
            workbook.Save("GetColumnOriginalWidthPointDemo.xlsx");
        }
    }
}
```

### Se även

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


