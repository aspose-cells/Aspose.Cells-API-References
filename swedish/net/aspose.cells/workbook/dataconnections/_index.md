---
title: "Workbook.DataConnections"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Workbook-egenskap. Hämtar samlingen ExternalConnection."
type: docs
url: /sv/net/aspose.cells/workbook/dataconnections/
---
## Workbook.DataConnections property

Hämtar [`ExternalConnection`](../../../aspose.cells.externalconnections/externalconnection/) samlingen.

```csharp
public ExternalConnectionCollection DataConnections { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorkbookPropertyDataConnectionsDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Skapa ett exempelark
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till data för att göra exemplet meningsfullt
            worksheet.Cells["A1"].Value = "Sample Data";

            try
            {
                // Åtkomst till egenskapen DataConnections
                var dataConnections = workbook.DataConnections;

                // Visa det aktuella värdet för egenskapen (läsoperation).
                Console.WriteLine("DataConnections count: " + dataConnections.Count);

                // Iterera genom anslutningarna om några finns.
                for (int i = 0; i < dataConnections.Count; i++)
                {
                    var connection = dataConnections[i];
                    Console.WriteLine($"Connection {i + 1}: {connection.Name}");
                }

                // Visa hur egenskapen påverkar beteendet
                Console.WriteLine("DataConnections has been demonstrated");

                // Spara resultatet
                workbook.Save("DataConnectionsDemo.xlsx");
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

* class [ExternalConnectionCollection](../../../aspose.cells.externalconnections/externalconnectioncollection/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


