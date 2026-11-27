---
title: "Worksheet.QueryTables"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Worksheet-egenskap. Hämtar QueryTableCollection i kalkylbladet"
type: docs
url: /sv/net/aspose.cells/worksheet/querytables/
---
## Worksheet.QueryTables property

Hämtar [`QueryTableCollection`](../../querytablecollection/) i kalkylbladet.

```csharp
public QueryTableCollection QueryTables { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyQueryTablesDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(2.5);
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B3"].PutValue(1.8);
            
            // Hämta den första frågetabellen (eftersom vi inte kan lägga till nya direkt)
            // Obs: QueryTables-samlingen är skrivskyddad i den här API-versionen
            if (worksheet.QueryTables.Count > 0)
            {
                QueryTable queryTable = worksheet.QueryTables[0];
                
                // Visa information om frågetabellen
                Console.WriteLine("Query Table Name: " + queryTable.Name);
                Console.WriteLine("Result Range: " + queryTable.ResultRange.Address);
                Console.WriteLine("Number of Query Tables: " + worksheet.QueryTables.Count);
            }
            else
            {
                Console.WriteLine("No query tables found in the worksheet.");
            }
            
            // Spara arbetsboken
            workbook.Save("QueryTableDemo.xlsx");
        }
    }
}
```

### Se även

* class [QueryTableCollection](../../querytablecollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


