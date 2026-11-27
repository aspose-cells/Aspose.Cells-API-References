---
title: "Cells.DeleteColumn"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cells-metoden. Raderar en kolumn"
type: docs
url: /sv/net/aspose.cells/cells/deletecolumn/
---
## DeleteColumn(int, bool) {#deletecolumn_1}

Tar bort en kolumn.

```csharp
public void DeleteColumn(int columnIndex, bool updateReference)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| columnIndex | Int32 | Index för kolumnen som ska raderas. |
| updateReference | Boolean | Indikerar om referenser ska uppdateras i andra kalkylblad. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodDeleteColumnWithInt32BooleanDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet
            Worksheet sheet = workbook.Worksheets[0];
            
            // Fyll i lite exempeldata i celler
            for (int i = 0; i < 5; i++)
            {
                for (int j = 0; j < 5; j++)
                {
                    sheet.Cells[i, j].PutValue($"Data {i},{j}");
                }
            }
            
            Console.WriteLine("Before deleting column:");
            PrintCellValues(sheet);
            
            // Radera den första kolumnen och flytta återstående kolumner åt vänster
            sheet.Cells.DeleteColumn(0, true);
            
            Console.WriteLine("\nAfter deleting column 0:");
            PrintCellValues(sheet);
            
            // Spara arbetsboken
            workbook.Save("DeleteColumnDemo.xlsx");
        }
        
        private static void PrintCellValues(Worksheet sheet)
        {
            for (int i = 0; i < 5; i++)
            {
                for (int j = 0; j < 5; j++)
                {
                    Console.Write(sheet.Cells[i, j].Value + "\t");
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

## DeleteColumn(int) {#deletecolumn}

Tar bort en kolumn.

```csharp
public void DeleteColumn(int columnIndex)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| columnIndex | Int32 | Index för kolumnen som ska raderas. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodDeleteColumnWithInt32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet sheet = workbook.Worksheets[0];
            
            // Fyll i lite exempeldata i kolumner
            Cells cells = sheet.Cells;
            cells["A1"].PutValue("Column A");
            cells["B1"].PutValue("Column B");
            cells["C1"].PutValue("Column C");
            
            // Radera kolumn vid index 1 (Kolumn B)
            cells.DeleteColumn(1);
            
            // Spara arbetsboken
            workbook.Save("output.xlsx");
            
            Console.WriteLine("Column deleted successfully.");
        }
    }
}
```

### Se även

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


