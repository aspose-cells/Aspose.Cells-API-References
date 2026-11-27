---
title: "Cells.GetRow"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cells-metod. Hämtar rad‑elementet vid det specificerade cellrad‑indexet"
type: docs
url: /sv/net/aspose.cells/cells/getrow/
---
## Cells.GetRow method

Hämtar [`Row`](../../row/) elementet på det angivna cellradindexet.

```csharp
[Obsolete("Use Cells.CheckRow(int row) instead.")]
public Row GetRow(int row)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| row | Int32 | Radindex |

### Returvärde

Om radobjektet finns, returnera Row-objektet, annars returnera null.

### Anmärkningar

OBS: Denna medlem är nu föråldrad. Använd istället Cells.CheckRow(int row)-metoden. Denna metod kommer att tas bort 12 månader senare från och med februari 2024. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodGetRowWithInt32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa celler i rad 5 för att säkerställa att raden finns
            worksheet.Cells["A5"].PutValue("Row 5 Data");
            worksheet.Cells["B5"].PutValue(12345);

            try
            {
                // Anropa GetRow-metoden med Int32-parameter
                Row resultRow = worksheet.Cells.GetRow(5);

                if (resultRow != null)
                {
                    // Demonstrera radmanipulation
                    resultRow.Height = 20;
                    Console.WriteLine($"Retrieved row 5 successfully. Current height: {resultRow.Height} points");
                    
                    // Räkna celler i raden
                    int cellCount = 0;
                    foreach (Cell cell in resultRow)
                    {
                        cellCount++;
                    }
                    Console.WriteLine($"Row 5 contains {cellCount} cells");
                }
                else
                {
                    Console.WriteLine("Row 5 not found in worksheet");
                }
            }
            catch (ArgumentOutOfRangeException ex)
            {
                Console.WriteLine($"Invalid row index: {ex.Message}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetRow: {ex.Message}");
            }

            // Spara den modifierade arbetsboken
            workbook.Save("CellsMethodGetRowWithInt32Demo.xlsx");
        }
    }
}
```

### Se även

* class [Row](../../row/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


