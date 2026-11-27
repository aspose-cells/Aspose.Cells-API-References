---
title: "QueryTable.Name"
second_title: "Aspose.Cells för .NET API‑referens"
description: "QueryTable-egenskap. Hämtar namnet på frågetabellen"
type: docs
url: /sv/net/aspose.cells/querytable/name/
---
## QueryTable.Name property

Hämtar namnet på querytable.

```csharp
public string Name { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class QueryTablePropertyNameDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för att simulera en frågetabell
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue("John");
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B3"].PutValue("Mary");

            try
            {
                // Kontrollera om det finns några frågetabeller i kalkylbladet
                if (worksheet.QueryTables.Count > 0)
                {
                    // Hämta den första frågetabellen
                    QueryTable queryTable = worksheet.QueryTables[0];

                    // Visa värdet för Name-egenskapen (skrivskyddad operation)
                    Console.WriteLine("Query Table Name: " + queryTable.Name);

                    // Visa andra skrivskyddade egenskaper för kontext
                    Console.WriteLine("Connection ID: " + queryTable.ConnectionId);
                    Console.WriteLine("Result Range: " + queryTable.ResultRange.Address);
                }
                else
                {
                    Console.WriteLine("No query tables found in the worksheet.");
                }

                // Spara arbetsboken
                workbook.Save("QueryTableNameDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [QueryTable](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


