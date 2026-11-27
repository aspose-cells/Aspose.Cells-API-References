---
title: "Cells.ExportTypeArray"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cells-metoden. Exporterar cellvärdestyp i Cells-samlingen till ett tvådimensionellt array‑objekt"
type: docs
url: /sv/net/aspose.cells/cells/exporttypearray/
---
## Cells.ExportTypeArray method

Exporterar cellvärdestyp i [`Cells`](../)-samlingen till ett tvådimensionellt array‑objekt.

```csharp
public CellValueType[] ExportTypeArray(int firstRow, int firstColumn, int totalRows, 
    int totalColumns)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| firstRow | Int32 | Radnumret för den första cellen som ska exporteras. |
| firstColumn | Int32 | Kolumnnumret för den första cellen som ska exporteras. |
| totalRows | Int32 | Antal rader som ska exporteras. |
| totalColumns | Int32 | Antal kolumner som ska exporteras. |

### Returvärde

Exporterad array-objekt som representerar cellvärdestyper.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodExportTypeArrayWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Ange värden i cells
            cells["A1"].PutValue(10);
            cells["B1"].PutValue("Hello");
            cells["A2"].PutValue(true);
            cells["B2"].PutValue(DateTime.Now);

            // Exportera celltyper till en 2D-array
            CellValueType[,] typeArray = cells.ExportTypeArray(0, 0, 2, 2);

            // Visa resultaten
            for (int i = 0; i < 2; i++)
            {
                for (int j = 0; j < 2; j++)
                {
                    Console.WriteLine($"Cell[{i},{j}] Type: {typeArray[i, j]}");
                }
            }

            // Visa exempel på undantag
            try
            {
                CellValueType[,] invalidArray = cells.ExportTypeArray(-1, 0, 2, 2);
            }
            catch (CellsException ex)
            {
                Console.WriteLine("Exception caught as expected: " + ex.Message);
            }
        }
    }
}
```

### Se även

* enum [CellValueType](../../cellvaluetype/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


