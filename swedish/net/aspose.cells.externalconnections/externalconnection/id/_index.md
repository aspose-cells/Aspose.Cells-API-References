---
title: "ExternalConnection.Id"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ExternalConnection egenskap. Hämtar id‑t för kopplingen"
type: docs
url: /sv/net/aspose.cells.externalconnections/externalconnection/id/
---
## ExternalConnection.Id property

Hämtar id för anslutningen.

```csharp
public int Id { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionPropertyIdDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            try
            {
                // Åtkomst till den första externa anslutningen (arbetsboken levereras med standardanslutningar)
                ExternalConnection connection = workbook.DataConnections[0];

                // Visa det aktuella Id‑värdet (skrivskyddad egenskap)
                Console.WriteLine("External Connection Id: " + connection.Id);

                // Visa andra skrivskyddade egenskaper för kontext
                Console.WriteLine("Connection Class Type: " + connection.ClassType);
                Console.WriteLine("Connection Name: " + connection.Name);

                // Spara arbetsboken
                workbook.Save("ExternalConnectionIdDemo.xlsx");
                Console.WriteLine("Workbook saved successfully with connection Id: " + connection.Id);
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

* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


