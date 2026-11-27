---
title: "UnionRange.Merge"
second_title: "Aspose.Cells för .NET API‑referens"
description: "UnionRange-metod. Kombinerar ett cellområde till en enda cell"
type: docs
url: /sv/net/aspose.cells/unionrange/merge/
---
## UnionRange.Merge method

Kombinerar ett cellområde till en enda cell.

```csharp
public void Merge()
```

### Anmärkningar

Referera till den sammanslagna cellen via adressen för den övre vänstra cellen i området.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class UnionRangeMethodMergeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Skapa ett cellområde (A1:B2)
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1", "B2");
            
            // Placera lite data i cellerna för att visualisera sammanslagning
            range[0, 0].PutValue("Before Merge");
            range[0, 1].PutValue("A1");
            range[1, 0].PutValue("B1");
            range[1, 1].PutValue("B2");
            
            try
            {
                // Skapa ett UnionRange från området
                UnionRange unionRange = worksheet.Cells.CreateRange("A1:B2").UnionRanges(new Aspose.Cells.Range[] { range });
                
                // Anropa Merge-metoden
                unionRange.Merge();
                
                // Placera värde i den sammanslagna cellen
                unionRange.PutValue("Merged A1:B2", true, true);
                
                Console.WriteLine("Cells merged successfully");
                
                // Avkommentera för att se effekten av att dela upp
                // unionRange.UnMerge();
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Merge method: {ex.Message}");
            }
            
            // Spara resultatet
            workbook.Save("MethodMergeDemo.xlsx");
        }
    }
}
```

### Se även

* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


