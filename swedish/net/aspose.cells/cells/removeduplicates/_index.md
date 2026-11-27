---
title: "Cells.RemoveDuplicates"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cells-metoden. Tar bort duplicerade rader i bladet"
type: docs
url: /sv/net/aspose.cells/cells/removeduplicates/
---
## RemoveDuplicates() {#removeduplicates}

Tar bort dubblett-rader i bladet.

```csharp
public void RemoveDuplicates()
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodRemoveDuplicatesDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;

            // Fyll celler med några duplicerade värden
            for (int i = 0; i < 10; i++)
            {
                for (int j = 0; j < 5; j++)
                {
                    // Skapa dubbletter i varannan rad
                    cells[i, j].PutValue(i % 2 == 0 ? "Duplicate" : $"Unique_{i}_{j}");
                }
            }

            Console.WriteLine($"Before RemoveDuplicates: {cells.Count} cells");
            
            // Ta bort duplicerade värden
            cells.RemoveDuplicates();

            Console.WriteLine($"After RemoveDuplicates: {cells.Count} cells");
        }
    }
}
```

### Se även

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## RemoveDuplicates(int, int, int, int) {#removeduplicates_1}

Tar bort dubblettvärden i området.

```csharp
public void RemoveDuplicates(int startRow, int startColumn, int endRow, int endColumn)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| startRow | Int32 | Startraden. |
| startColumn | Int32 | Startkolumnen |
| endRow | Int32 | Slutradens index. |
| endColumn | Int32 | Slutkolumnens index. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodRemoveDuplicatesWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Lägg till exempeldata med dubbletter
            cells["A1"].PutValue("Apple");
            cells["A2"].PutValue("Orange");
            cells["A3"].PutValue("Apple");
            cells["A4"].PutValue("Banana");
            cells["A5"].PutValue("Orange");

            // Ta bort dubbletter från kolumn A (0-baserat index)
            cells.RemoveDuplicates(0, 0, 5, 0);

            // Spara arbetsboken
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## RemoveDuplicates(int, int, int, int, bool, int[]) {#removeduplicates_2}

Tar bort dubblettdata i området.

```csharp
public void RemoveDuplicates(int startRow, int startColumn, int endRow, int endColumn, 
    bool hasHeaders, int[] columnOffsets)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| startRow | Int32 | Startraden. |
| startColumn | Int32 | Startkolumnen |
| endRow | Int32 | Slutradens index. |
| endColumn | Int32 | Slutkolumnens index. |
| hasHeaders | Boolean | Indikerar om intervallet innehåller rubriker. |
| columnOffsets | Int32[] | Kolumnförskjutningarna. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodRemoveDuplicatesWithInt32Int32Int32Int32BooleanIntDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Fyll i exempeldata med dubbletter
            cells[0, 0].PutValue("ID");
            cells[0, 1].PutValue("Name");
            cells[0, 2].PutValue("Age");
            
            cells[1, 0].PutValue(1);
            cells[1, 1].PutValue("John");
            cells[1, 2].PutValue(30);

            cells[2, 0].PutValue(2);
            cells[2, 1].PutValue("Jane");
            cells[2, 2].PutValue(25);

            cells[3, 0].PutValue(1); // Duplicate ID
            cells[3, 1].PutValue("John"); // Duplicate Name
            cells[3, 2].PutValue(35);

            cells[4, 0].PutValue(3);
            cells[4, 1].PutValue("Bob");
            cells[4, 2].PutValue(40);

            try
            {
                // Ta bort dubbletter från rader 1-4 (0-baserade), kolumner 0-2
                // Kontrollera dubbletter baserat på de två första kolumnerna (ID och Namn)
                cells.RemoveDuplicates(1, 0, 4, 2, true, new int[] { 0, 1 });

                Console.WriteLine("Duplicates removed successfully. Remaining rows: " + (cells.MaxDataRow + 1));
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing RemoveDuplicates method: {ex.Message}");
            }

            // Spara resultatet
            workbook.Save("RemoveDuplicatesDemo.xlsx");
        }
    }
}
```

### Se även

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


