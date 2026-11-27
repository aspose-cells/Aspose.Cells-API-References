---
title: "QueryTable.ConnectionId"
second_title: "Aspose.Cells för .NET API‑referens"
description: "QueryTable-egenskap. Hämtar anslutnings‑id för frågetabellen"
type: docs
url: /sv/net/aspose.cells/querytable/connectionid/
---
## QueryTable.ConnectionId property

Hämtar anslutnings‑id för frågetabellen.

```csharp
public int ConnectionId { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class QueryTablePropertyConnectionIdDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för att simulera ett frågetabells scenario
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue("Sample Data");

            try
            {
                // Kontrollera om det finns några frågetabeller i kalkylbladet
                if (worksheet.QueryTables.Count > 0)
                {
                    // Hämta den första frågetabellen
                    QueryTable queryTable = worksheet.QueryTables[0];

                    // Visa ConnectionId‑egenskapens värde (skrivskyddad)
                    Console.WriteLine("Query Table ConnectionId: " + queryTable.ConnectionId);

                    // Visa andra relaterade egenskaper för kontext
                    Console.WriteLine("Query Table Name: " + queryTable.Name);
                    Console.WriteLine("External Connection: " +
                        (queryTable.ExternalConnection != null ? queryTable.ExternalConnection.Name : "None"));
                }
                else
                {
                    Console.WriteLine("No query tables found in the worksheet.");
                }

                // Spara arbetsboken
                workbook.Save("ConnectionIdDemo.xlsx");
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


