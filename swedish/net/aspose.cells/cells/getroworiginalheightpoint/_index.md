---
title: "Cells.GetRowOriginalHeightPoint"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cells-metoden. Hämtar originalhöjden för rader i enheten punkt om raden är dold"
type: docs
url: /sv/net/aspose.cells/cells/getroworiginalheightpoint/
---
## Cells.GetRowOriginalHeightPoint method

Hämtar originalhöjden för raden i enheten punkt om raden är dold

```csharp
[Obsolete("Use Cells.GetRowHeight(int,bool,CellsUnitType) method, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public double GetRowOriginalHeightPoint(int row)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| row | Int32 | Radindexet. |

### Anmärkningar

OBS: Denna medlem är nu föråldrad. Använd istället Cells.GetRowHeight(int,bool,CellsUnitType)-metoden. Denna metod kommer att tas bort 12 månader senare från och med april 2024. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodGetRowOriginalHeightPointWithInt32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Spara originalhöjden innan ändring
            double originalHeightBefore = cells.GetRowOriginalHeightPoint(0);
            
            // Ändra radens höjd
            cells.SetRowHeight(0, 25.5);

            try
            {
                // Hämta originalhöjden efter ändring
                double originalHeight = cells.GetRowOriginalHeightPoint(0);
                double currentHeight = cells.GetRowHeight(0);

                Console.WriteLine($"Original row height: {originalHeight} points");
                Console.WriteLine($"Current row height: {currentHeight} points");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetRowOriginalHeightPoint: {ex.Message}");
            }

            workbook.Save("GetRowOriginalHeightPointDemo.xlsx");
        }
    }
}
```

### Se även

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


