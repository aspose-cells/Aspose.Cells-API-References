---
title: "WorksheetCollection.GetRangeByName"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WorksheetCollection-metod. Hämtar Range‑objektet efter fördefinierat namn"
type: docs
url: /sv/net/aspose.cells/worksheetcollection/getrangebyname/
---
## GetRangeByName(string) {#getrangebyname}

Hämtar Range‑objektet efter fördefinierat namn.

```csharp
public Range GetRangeByName(string rangeName)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rangeName | String | Namn på intervallet. |

### Returvärde

Range‑objekt.

Returnerar null om det namngivna området inte finns.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodGetRangeByNameWithStringDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till lite data i cellerna
            worksheet.Cells["A1"].PutValue("Apple");
            worksheet.Cells["B1"].PutValue("Banana");
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["B2"].PutValue(200);
            
            // Skapa ett namngivet område
            worksheet.Cells.CreateRange("A1:B2").Name = "FruitData";
            
            // Hämta det namngivna intervallet med GetRangeByName
            Aspose.Cells.Range namedRange = workbook.Worksheets.GetRangeByName("FruitData");
            
            // Visa intervallinformation om den hittas
            if (namedRange != null)
            {
                Console.WriteLine("Range found: " + namedRange.Address);
                Console.WriteLine("First cell value: " + namedRange[0, 0].StringValue);
            }
            else
            {
                Console.WriteLine("Range not found");
            }
        }
    }
}
```

### Se även

* class [Range](../../range/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetRangeByName(string, int, bool) {#getrangebyname_1}

Hämtar [`Range`](../../range/) efter fördefinierat namn eller tabellens namn

```csharp
public Range GetRangeByName(string rangeName, int currentSheetIndex, bool includeTable)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rangeName | String | Namn på intervallet eller tabellens namn. |
| currentSheetIndex | Int32 | Bladindexet. -1 representerar globalt. |
| includeTable | Boolean | Indikerar om alla tabeller ska kontrolleras. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorksheetCollectionMethodGetRangeByNameWithStringInt32BooleanDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Skapa ett namngivet område
            Aspose.Cells.Range namedRange = worksheet.Cells.CreateRange("A1", "C3");
            namedRange.Name = "TestRange";
            
            // Lägg till data i intervallet
            for (int i = 0; i < 3; i++)
            {
                for (int j = 0; j < 3; j++)
                {
                    worksheet.Cells[i, j].PutValue($"Cell {i+1},{j+1}");
                }
            }

            try
            {
                // Anropa GetRangeByName med parametrarna (String, Int32, Boolean)
                Aspose.Cells.Range retrievedRange = workbook.Worksheets.GetRangeByName("TestRange", 0, true);
                
                Console.WriteLine("Method executed successfully with parameters (String, Int32, Boolean)");
                Console.WriteLine($"Retrieved range address: {retrievedRange.Address}");
                Console.WriteLine($"Range contains {retrievedRange.RowCount} rows and {retrievedRange.ColumnCount} columns");
                
                // Visa intervallevärden
                Console.WriteLine("Range values:");
                foreach (Cell cell in retrievedRange)
                {
                    Console.WriteLine($"{cell.Name}: {cell.Value}");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetRangeByName method: {ex.Message}");
            }
            
            // Spara resultatet
            workbook.Save("WorksheetCollectionMethodGetRangeByNameDemo.xlsx");
        }
    }
}
```

### Se även

* class [Range](../../range/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


