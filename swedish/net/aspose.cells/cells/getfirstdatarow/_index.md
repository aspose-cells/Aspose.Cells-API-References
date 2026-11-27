---
title: "Cells.GetFirstDataRow"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cells-metod. Hämtar det första radindexet för cellen som innehåller data i den angivna kolumnen"
type: docs
url: /sv/net/aspose.cells/cells/getfirstdatarow/
---
## Cells.GetFirstDataRow method

Hämtar det första radindexet för cellen som innehåller data i den angivna kolumnen.

```csharp
public int GetFirstDataRow(int column)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| column | Int32 | Kolumnindex. |

### Returvärde

första radens index.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodGetFirstDataRowWithInt32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till lite exempeldata för att demonstrera metoden
            worksheet.Cells["A1"].Value = "Header";
            worksheet.Cells["A2"].Value = "Data1";
            worksheet.Cells["A3"].Value = "Data2";
            worksheet.Cells["B5"].Value = "Data3";
            worksheet.Cells["C7"].Value = "Data4";

            try
            {
                // Hämta Cells-samlingen från kalkylbladet
                Cells cells = worksheet.Cells;

                // Anropa GetFirstDataRow för kolumn A (index 0)
                int firstDataRowA = cells.GetFirstDataRow(0);
                Console.WriteLine($"First data row in column A: {firstDataRowA}");

                // Anropa GetFirstDataRow för kolumn B (index 1)
                int firstDataRowB = cells.GetFirstDataRow(1);
                Console.WriteLine($"First data row in column B: {firstDataRowB}");

                // Anropa GetFirstDataRow för kolumn C (index 2)
                int firstDataRowC = cells.GetFirstDataRow(2);
                Console.WriteLine($"First data row in column C: {firstDataRowC}");

                // Spara arbetsboken
                workbook.Save("GetFirstDataRowDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


