---
title: "Cells.DeleteRows"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cells-metod. Raderar flera rader"
type: docs
url: /sv/net/aspose.cells/cells/deleterows/
---
## DeleteRows(int, int) {#deleterows}

Tar bort flera rader.

```csharp
public bool DeleteRows(int rowIndex, int totalRows)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rowIndex | Int32 | Det första radindexet som ska raderas. |
| totalRows | Int32 | Antal rader som ska raderas. |

### Anmärkningar

Om det borttagna intervallet innehåller den övre delen (inte hela) av tabellen (ListObject), kan intervallet inte tas bort och inget görs. Det fungerar på samma sätt som i MS Excel.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodDeleteRowsWithInt32Int32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Fyll i lite exempeldata
            for (int i = 0; i < 10; i++)
            {
                for (int j = 0; j < 5; j++)
                {
                    cells[i, j].PutValue($"Row {i+1}, Col {j+1}");
                }
            }

            Console.WriteLine("Before deleting rows:");
            PrintCellValues(cells, 0, 9, 0, 4);

            // Ta bort 2 rader med start från radindex 2 (3:e raden)
            cells.DeleteRows(2, 2);

            Console.WriteLine("\nAfter deleting rows 3-4:");
            PrintCellValues(cells, 0, 7, 0, 4);

            // Spara arbetsboken
            workbook.Save("output.xlsx");
        }

        private static void PrintCellValues(Cells cells, int startRow, int endRow, int startCol, int endCol)
        {
            for (int i = startRow; i <= endRow; i++)
            {
                for (int j = startCol; j <= endCol; j++)
                {
                    Console.Write($"{cells[i, j].StringValue}\t");
                }
                Console.WriteLine();
            }
        }
    }
}
```

### Se även

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## DeleteRows(int, int, bool) {#deleterows_2}

Tar bort flera rader i kalkylbladet.

```csharp
public bool DeleteRows(int rowIndex, int totalRows, bool updateReference)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rowIndex | Int32 | Index för den första raden som ska raderas. |
| totalRows | Int32 | Antal rader som ska raderas. |
| updateReference | Boolean | Indikerar om referenser ska uppdateras i andra kalkylblad. |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class CellsMethodDeleteRowsWithInt32Int32BooleanDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Importera data till celler
            worksheet.Cells.ImportTwoDimensionArray(new object[2, 2] { { "A1", "B1" }, { "A2", "B2" } }, 0, 0);

            // Skapa en tabell
            ListObject table = worksheet.ListObjects[worksheet.ListObjects.Add(0, 0, 1, 1, false)];
            table.ShowHeaderRow = false;

            Console.WriteLine("Before DeleteRows:");
            Console.WriteLine($"Table Data Range Row Count: {table.ListColumns.Count}");
            Console.WriteLine($"Table Start Row: {table.StartRow}");
            Console.WriteLine($"Table End Row: {table.EndRow}");

            // Ta bort rad på index 1 (andra raden) med uppdateringsreferens
            worksheet.Cells.DeleteRows(1, 1, true);

            Console.WriteLine("\nAfter DeleteRows:");
            Console.WriteLine($"Table Data Range Row Count: {table.ListColumns.Count}");
            Console.WriteLine($"Table Start Row: {table.StartRow}");
            Console.WriteLine($"Table End Row: {table.EndRow}");
        }
    }
}
```

### Se även

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## DeleteRows(int, int, DeleteOptions) {#deleterows_1}

Tar bort flera rader i kalkylbladet.

```csharp
public bool DeleteRows(int rowIndex, int totalRows, DeleteOptions options)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rowIndex | Int32 | Index för den första raden som ska raderas. |
| totalRows | Int32 | Antal rader som ska raderas. |
| alternativ | DeleteOptions | Alternativ för raderingsoperationen |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodDeleteRowsWithInt32Int32DeleteOptionsDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;

            // Ange exempeldata och formler
            cells["A1"].PutValue(10);
            cells["A2"].PutValue(20);
            cells["A3"].PutValue(30);
            cells["B1"].Formula = "=SUM(A1:A3)";
            
            // Ta bort rad 2 utan övervakning (eftersom FormulaChangeMonitor inte är tillgänglig)
            cells.DeleteRows(1, 1, new DeleteOptions());
            
            Console.WriteLine("Deleted row 2. Formula in B1 should now be: " + cells["B1"].Formula);
        }
    }
}
```

### Se även

* class [DeleteOptions](../../deleteoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


