---
title: "QueryTable.ExternalConnection"
second_title: "Aspose.Cells för .NET API‑referens"
description: "QueryTable-egenskap. Hämtar den relaterade externa anslutningen"
type: docs
url: /sv/net/aspose.cells/querytable/externalconnection/
---
## QueryTable.ExternalConnection property

Hämtar den relaterade externa anslutningen.

```csharp
public ExternalConnection ExternalConnection { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class QueryTablePropertyExternalConnectionDemo
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

                    // Åtkomst till ExternalConnection-egenskapen (skrivskyddad)
                    ExternalConnection externalConnection = queryTable.ExternalConnection;

                    // Visa information om den externa anslutningen
                    if (externalConnection != null)
                    {
                        Console.WriteLine("External Connection ID: " + externalConnection.Id);
                        Console.WriteLine("External Connection Name: " + externalConnection.Name);
                        Console.WriteLine("External Connection Type: " + externalConnection.ClassType);
                        Console.WriteLine("Connection String: " + externalConnection.ConnectionString);
                        Console.WriteLine("Refresh on Load: " + externalConnection.RefreshOnLoad);
                    }
                    else
                    {
                        Console.WriteLine("No external connection associated with this query table.");
                    }

                    // Visa andra frågetabellsegenskaper för kontext
                    Console.WriteLine("Query Table Name: " + queryTable.Name);
                    Console.WriteLine("Connection ID: " + queryTable.ConnectionId);
                }
                else
                {
                    Console.WriteLine("No query tables found in the worksheet.");
                }

                // Spara arbetsboken
                workbook.Save("ExternalConnectionDemo.xlsx");
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

* class [ExternalConnection](../../../aspose.cells.externalconnections/externalconnection/)
* class [QueryTable](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


