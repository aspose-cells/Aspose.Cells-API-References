---
title: "Cells.DeleteRow"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cells-metod. Raderar en rad"
type: docs
url: /sv/net/aspose.cells/cells/deleterow/
---
## DeleteRow(int) {#deleterow}

Tar bort en rad.

```csharp
public void DeleteRow(int rowIndex)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rowIndex | Int32 | Index för raden som ska raderas. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodDeleteRowWithInt32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;

            // Ställ in en delad formel i rad 66
            cells[65, 0].SetSharedFormula("=SUM(B10:B66)", 1, 6);

            // Ta bort rad 9 (vilket kommer att flytta raderna uppåt)
            cells.DeleteRow(9);

            // Verifiera att formeln justerades efter radraderingen
            for (int i = 1; i < 7; i++)
            {
                char columnName = (char)('A' + i);
                Console.WriteLine($"Cell {columnName}66 formula after deletion: {cells[64, i].Formula}");
            }

            // Ta bort raderna 60-61 (vilket kommer att flytta raderna uppåt)
            cells.DeleteRows(59, 2);

            // Verifiera att formeln justerades efter radernas borttagning
            for (int i = 1; i < 7; i++)
            {
                char columnName = (char)('A' + i);
                Console.WriteLine($"Cell {columnName}64 formula after deletion: {cells[62, i].Formula}");
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

## DeleteRow(int, bool) {#deleterow_1}

Tar bort en rad.

```csharp
public void DeleteRow(int rowIndex, bool updateReference)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rowIndex | Int32 | Index för raden som ska raderas. |
| updateReference | Boolean | Indikerar om referenser ska uppdateras i andra kalkylblad. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodDeleteRowWithInt32BooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            sheet.Cells["A1"].PutValue("Item");
            sheet.Cells["A2"].PutValue("Apple");
            sheet.Cells["A3"].PutValue("Banana");
            sheet.Cells["A4"].PutValue("Cherry");

            Console.WriteLine("Original Data:");
            for (int i = 1; i <= 4; i++)
            {
                Console.WriteLine(sheet.Cells[$"A{i}"].Value);
            }

            sheet.Cells.DeleteRow(2, true);

            Console.WriteLine("\nData After Deletion:");
            for (int i = 1; i <= 3; i++)
            {
                Console.WriteLine(sheet.Cells[$"A{i}"].Value);
            }

            workbook.Save("DeleteRowExample.xlsx");
        }
    }
}
```

### Se även

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


