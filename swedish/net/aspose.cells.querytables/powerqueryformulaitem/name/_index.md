---
title: "PowerQueryFormulaItem.Name"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PowerQueryFormulaItem egenskap. Hämtar namnet på objektet"
type: docs
url: /sv/net/aspose.cells.querytables/powerqueryformulaitem/name/
---
## PowerQueryFormulaItem.Name property

Hämtar namnet på objektet.

```csharp
public string Name { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PowerQueryFormulaItemPropertyNameDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata för Power Query
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Laptop");
            worksheet.Cells["B2"].PutValue(1200);
            
            // Spara för att utlösa skapandet av Power Query
            string sourcePath = "pq_source.xlsx";
            workbook.Save(sourcePath);
            
            // Öppna igen för att komma åt Power Query-formler
            workbook = new Workbook(sourcePath);
            Aspose.Cells.QueryTables.DataMashup mashupData = workbook.DataMashup;
            
            // Bearbeta Power Query-formler
            foreach (Aspose.Cells.QueryTables.PowerQueryFormula formula in mashupData.PowerQueryFormulas)
            {
                Console.WriteLine("Formula Name: " + formula.Name);
                
                foreach (Aspose.Cells.QueryTables.PowerQueryFormulaItem item in formula.PowerQueryFormulaItems)
                {
                    Console.WriteLine("  Item Name: " + item.Name);
                    
                    // Demonstrera användning av Name‑egenskapen
                    if (item.Name == "Source")
                    {
                        Console.WriteLine("Original Value: " + item.Value);
                        item.Value = "ModifiedSource";
                        Console.WriteLine("Modified Value: " + item.Value);
                    }
                }
            }
            
            // Spara modifierad arbetsbok
            workbook.Save("pq_modified.xlsx");
        }
    }
}
```

### Se även

* class [PowerQueryFormulaItem](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


