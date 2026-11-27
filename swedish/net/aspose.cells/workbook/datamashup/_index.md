---
title: "Workbook.DataMashup"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Workbook-egenskap. Hämtar mashup-data"
type: docs
url: /sv/net/aspose.cells/workbook/datamashup/
---
## Workbook.DataMashup property

Hämtar mashup-data.

```csharp
public DataMashup DataMashup { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.ExternalConnections;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyDataMashupDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata för att utlösa Power Query
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B3"].PutValue(150);

            // Spara till en fil
            string sourcePath = "source.xlsx";
            workbook.Save(sourcePath);

            // Öppna arbetsboken igen för att komma åt DataMashup
            workbook = new Workbook(sourcePath);
            
            // Kom åt Power Query-formler via DataMashup-egenskapen
            var queries = workbook.DataMashup.PowerQueryFormulas;
            
            // Skriv ut grundläggande information om frågor
            Console.WriteLine($"Number of Power Query formulas: {queries.Count}");
            
            // Om det finns några frågor, visa detaljer för den första
            if (queries.Count > 0)
            {
                foreach (var query in queries)
                {
                    Console.WriteLine($"Query Name: {query.Name}");
                    Console.WriteLine($"Number of items: {query.PowerQueryFormulaItems.Count}");
                    break; // Just show first query for demo
                }
            }

            // Spara till en ny fil
            string destPath = "output.xlsx";
            workbook.Save(destPath);
        }
    }
}
```

### Se även

* class [DataMashup](../../../aspose.cells.querytables/datamashup/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


