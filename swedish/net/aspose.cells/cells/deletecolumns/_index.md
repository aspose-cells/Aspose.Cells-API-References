---
title: "Cells.DeleteColumns"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cells-metoden. Tar bort flera kolumner"
type: docs
url: /sv/net/aspose.cells/cells/deletecolumns/
---
## DeleteColumns(int, int, bool) {#deletecolumns_1}

Tar bort flera kolumner.

```csharp
public void DeleteColumns(int columnIndex, int totalColumns, bool updateReference)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| columnIndex | Int32 | Index för den första kolumnen som ska tas bort. |
| totalColumns | Int32 | Antal kolumner som ska tas bort. |
| updateReference | Boolean | Indikerar om referenser ska uppdateras i andra kalkylblad. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodDeleteColumnsWithInt32Int32BooleanDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata i celler
            worksheet.Cells["A1"].PutValue("Column 1");
            worksheet.Cells["B1"].PutValue("Column 2");
            worksheet.Cells["C1"].PutValue("Column 3");
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["B2"].PutValue(200);
            worksheet.Cells["C2"].PutValue(300);

            // Lägg till en formel som refererar till dessa kolumner
            worksheet.Cells["D1"].Formula = "=SUM(A2:C2)";

            Console.WriteLine("Before deleting columns:");
            Console.WriteLine("A1: " + worksheet.Cells["A1"].Value);
            Console.WriteLine("B1: " + worksheet.Cells["B1"].Value);
            Console.WriteLine("C1: " + worksheet.Cells["C1"].Value);
            Console.WriteLine("D1 formula: " + worksheet.Cells["D1"].Formula);

            // Ta bort kolumn B (index 1) och flytta återstående kolumner åt vänster
            worksheet.Cells.DeleteColumns(1, 1, true);

            Console.WriteLine("\nAfter deleting column B:");
            Console.WriteLine("A1: " + worksheet.Cells["A1"].Value);
            Console.WriteLine("B1: " + worksheet.Cells["B1"].Value);
            Console.WriteLine("C1 formula: " + worksheet.Cells["C1"].Formula);
        }
    }
}
```

### Se även

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## DeleteColumns(int, int, DeleteOptions) {#deletecolumns}

Tar bort flera kolumner.

```csharp
public void DeleteColumns(int columnIndex, int totalColumns, DeleteOptions options)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| columnIndex | Int32 | Index för den första kolumnen som ska tas bort. |
| totalColumns | Int32 | Antal kolumner som ska tas bort. |
| alternativ | DeleteOptions | Alternativ för raderingsoperationen |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodDeleteColumnsWithInt32Int32DeleteOptionsDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fyll i exempeldata i kolumnerna A-E
            for (int col = 0; col < 5; col++)
            {
                worksheet.Cells[0, col].Value = $"Column {(char)('A' + col)}";
                worksheet.Cells[1, col].Value = $"Data{col + 1}";
            }

            // Skapa DeleteOptions och konfigurera inställningarna
            DeleteOptions options = new DeleteOptions
            {
                UpdateReference = true // Update references in other cells
            };

            try
            {
                // Ta bort 2 kolumner med start från kolumn B (index 1)
                worksheet.Cells.DeleteColumns(1, 2, options);
                
                Console.WriteLine("Deleted columns B and C successfully");
                
                // Visa återstående data i kolumn B (ursprungliga kolumn D)
                Console.WriteLine($"New column B value: {worksheet.Cells[1, 1].StringValue}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing DeleteColumns: {ex.Message}");
            }
            
            // Spara den modifierade arbetsboken
            workbook.Save("DeleteColumnsWithOptionsDemo.xlsx");
        }
    }
}
```

### Se även

* class [DeleteOptions](../../deleteoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


