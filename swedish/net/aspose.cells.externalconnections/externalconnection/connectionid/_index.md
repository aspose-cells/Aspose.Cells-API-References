---
title: "ExternalConnection.ConnectionId"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ExternalConnection-egenskap. Anger det unika identifieraren för denna anslutning"
type: docs
url: /sv/net/aspose.cells.externalconnections/externalconnection/connectionid/
---
## ExternalConnection.ConnectionId property

Anger det unika identifieraren för denna anslutning.

```csharp
[Obsolete("Use ExternalConnection.Id property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int ConnectionId { get; }
```

### Anmärkningar

OBS: Denna egenskap är nu föråldrad. Använd istället ExternalConnection.Id-egenskap. Denna egenskap kommer att tas bort 12 månader senare från och med oktober 2024. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionPropertyConnectionIdDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            try
            {
                // Åtkomst till den första externa anslutningen (arbetsboken levereras med standardanslutningar)
                ExternalConnection connection = workbook.DataConnections[0];

                // Visa ConnectionId-värdet (skrivskyddad egenskap)
                Console.WriteLine("ConnectionId value: " + connection.ConnectionId);

                // Visa Id-värdet för jämförelse (också skrivskyddad)
                Console.WriteLine("Id value: " + connection.Id);

                // Visa att båda egenskaperna är skrivskyddade genom att försöka visa dem
                Console.WriteLine("ConnectionId and Id are both read-only properties");
                Console.WriteLine("ConnectionId: " + connection.ConnectionId + ", Id: " + connection.Id);

                // Spara arbetsboken
                workbook.Save("ConnectionIdDemo.xlsx");
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


