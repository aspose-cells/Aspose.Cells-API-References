---
title: "Cells.ExportArray"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cells-metod. Exporterar data i Cells-samlingen till ett tvådimensionellt array‑objekt"
type: docs
url: /sv/net/aspose.cells/cells/exportarray/
---
## Cells.ExportArray method

Exporterar data i [`Cells`](../)-samlingen till ett tvådimensionellt array‑objekt.

```csharp
public object[] ExportArray(int firstRow, int firstColumn, int totalRows, int totalColumns)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| firstRow | Int32 | Radnumret för den första cellen som ska exporteras. |
| firstColumn | Int32 | Kolumnnumret för den första cellen som ska exporteras. |
| totalRows | Int32 | Antal rader som ska exporteras |
| totalColumns | Int32 | Antal kolumner som ska exporteras |

### Returvärde

Exporterad cellvärde‑array‑objekt.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodExportArrayWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Fyll i lite exempeldata
            cells[0, 0].PutValue("A");
            cells[0, 1].PutValue("B");
            cells[1, 0].PutValue(10);
            cells[1, 1].PutValue(20);

            try
            {
                // Exportera data till array
                object[,] dataArray = cells.ExportArray(0, 0, 2, 2);
                
                // Visa den exporterade arrayen
                for (int i = 0; i < 2; i++)
                {
                    for (int j = 0; j < 2; j++)
                    {
                        Console.Write(dataArray[i, j] + "\t");
                    }
                    Console.WriteLine();
                }
            }
            catch (CellsException ex)
            {
                Console.WriteLine("Error exporting array: " + ex.Message);
            }
        }
    }
}
```

### Se även

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


