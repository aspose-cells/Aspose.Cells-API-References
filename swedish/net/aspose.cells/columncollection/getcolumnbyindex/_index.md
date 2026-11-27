---
title: "ColumnCollection.GetColumnByIndex"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ColumnCollection‑metod. Hämtar Column‑objektet efter positionen i listan"
type: docs
url: /sv/net/aspose.cells/columncollection/getcolumnbyindex/
---
## ColumnCollection.GetColumnByIndex method

Hämtar [`Column`](../../column/)‑objektet efter positionen i listan.

```csharp
public Column GetColumnByIndex(int index)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | Int32 | Positionen i listan. |

### Returvärde

Returnerar kolumnobjektet.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ColumnCollectionMethodGetColumnByIndexWithInt32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok och öppna det första kalkylbladet
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata i kolumn A
            worksheet.Cells["A1"].Value = "Aspose.Cells Column Demo";

            try
            {
                // Hämta referens till kolumnsamling
                ColumnCollection columns = worksheet.Cells.Columns;

                // Åtkomst till kolumn på index 0 (kolumn A) med GetColumnByIndex
                Column column = columns.GetColumnByIndex(0);

                // Ändra kolumnbredd för att demonstrera kolumnåtkomst
                column.Width = 25;

                Console.WriteLine("Modified width of column at index 0 (Column A) to 25 characters.");
            }
            catch (ArgumentOutOfRangeException ex)
            {
                Console.WriteLine($"Invalid column index: {ex.Message}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }

            // Spara den modifierade arbetsboken
            workbook.Save("ColumnCollectionMethodGetColumnByIndexWithInt32Demo.xlsx");
        }
    }
}
```

### Se även

* class [Column](../../column/)
* class [ColumnCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


