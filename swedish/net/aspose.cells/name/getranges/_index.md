---
title: "Name.GetRanges"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Name-metod. Hämtar alla områden som refereras av detta namn"
type: docs
url: /sv/net/aspose.cells/name/getranges/
---
## GetRanges() {#getranges}

Hämtar alla områden som refereras av detta namn.

```csharp
public Range[] GetRanges()
```

### Returvärde

Alla områden.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NameMethodGetRangesDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till lite exempeldata
            worksheet.Cells["A1"].PutValue("Apple");
            worksheet.Cells["A2"].PutValue("Banana");
            worksheet.Cells["A3"].PutValue("Cherry");
            
            // Skapa ett namngivet område
            int index = workbook.Worksheets.Names.Add("Fruits");
            Name name = workbook.Worksheets.Names[index];
            name.RefersTo = "=Sheet1!$A$1:$A$3";
            
            // Hämta områden med omräkning
            Aspose.Cells.Range[] ranges1 = name.GetRanges();
            Console.WriteLine("Ranges with recalculation:");
            PrintRanges(ranges1);
            
            // Hämta områden utan omräkning
            Aspose.Cells.Range[] ranges2 = name.GetRanges(false);
            Console.WriteLine("\nRanges without recalculation:");
            PrintRanges(ranges2);
        }
        
        private static void PrintRanges(Aspose.Cells.Range[] ranges)
        {
            if (ranges != null)
            {
                foreach (Aspose.Cells.Range range in ranges)
                {
                    Console.WriteLine($"Range: {range.Address}");
                }
            }
            else
            {
                Console.WriteLine("No ranges found");
            }
        }
    }
}
```

### Se även

* class [Range](../../range/)
* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetRanges(bool) {#getranges_1}

Hämtar alla områden som refereras av detta namn.

```csharp
public Range[] GetRanges(bool recalculate)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| omräkna | Boolean | om det ska omräknas om detta namn redan har beräknats före detta anrop. |

### Returvärde

Alla områden.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NameMethodGetRangesWithBooleanDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till lite exempeldata
            worksheet.Cells["A1"].PutValue("Test");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(20);
            
            // Skapa ett namngivet område
            int index = workbook.Worksheets.Names.Add("TestRange");
            Name namedRange = workbook.Worksheets.Names[index];
            namedRange.RefersTo = "=Sheet1!$A$1:$A$3";
            
            // Hämta områden utan att beräkna om
            Aspose.Cells.Range[] ranges1 = namedRange.GetRanges(false);
            Console.WriteLine("Ranges count (no recalc): " + ranges1.Length);
            
            // Hämta områden med omberäkning
            Aspose.Cells.Range[] ranges2 = namedRange.GetRanges();
            Console.WriteLine("Ranges count (with recalc): " + ranges2.Length);
            
            // Ändra området och demonstrera omberäkning
            worksheet.Cells["A4"].PutValue(30);
            namedRange.RefersTo = "=Sheet1!$A$1:$A$4";
            
            // Hämta områden med och utan omberäkning efter ändring
            Aspose.Cells.Range[] ranges3 = namedRange.GetRanges(false);
            Console.WriteLine("Ranges count after mod (no recalc): " + ranges3.Length);
            
            Aspose.Cells.Range[] ranges4 = namedRange.GetRanges();
            Console.WriteLine("Ranges count after mod (with recalc): " + ranges4.Length);
        }
    }
}
```

### Se även

* class [Range](../../range/)
* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


