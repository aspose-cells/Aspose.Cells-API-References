---
title: "UnionRange.UnMerge"
second_title: "Aspose.Cells för .NET API‑referens"
description: "UnionRange-metod. Avslår sammanslagna celler i detta område"
type: docs
url: /sv/net/aspose.cells/unionrange/unmerge/
---
## UnionRange.UnMerge method

Avslår sammanslagna celler i detta område.

```csharp
public void UnMerge()
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class UnionRangeMethodUnMergeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Skapa ett område och slå ihop celler
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1", "B2");
            UnionRange unionRange = worksheet.Cells.CreateRange("A1:B2").UnionRanges(new Aspose.Cells.Range[] { range });
            
            // Slå ihop cellerna och lägg in ett värde
            unionRange.Merge();
            unionRange.PutValue("Merged Cells", true, true);
            
            try
            {
                // Anropa UnMerge-metoden
                unionRange.UnMerge();
                
                Console.WriteLine("Cells unmerged successfully");
                
                // Sätt värden i de avsammanfogade cellerna för att demonstrera effekten
                worksheet.Cells["A1"].PutValue("A1");
                worksheet.Cells["A2"].PutValue("A2");
                worksheet.Cells["B1"].PutValue("B1");
                worksheet.Cells["B2"].PutValue("B2");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing UnMerge method: {ex.Message}");
            }
            
            // Spara resultatet
            workbook.Save("MethodUnMergeDemo.xlsx");
        }
    }
}
```

### Se även

* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


