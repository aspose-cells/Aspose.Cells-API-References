---
title: "ExternalConnection.BackgroundRefresh"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ExternalConnection-egenskap. Anger om anslutningen kan uppdateras i bakgrunden asynkront. true om föredragen användning av anslutningen är att uppdatera asynkront i bakgrunden, false om föredragen användning av anslutningen är att uppdatera synkront i förgrunden."
type: docs
url: /sv/net/aspose.cells.externalconnections/externalconnection/backgroundrefresh/
---
## ExternalConnection.BackgroundRefresh property

Anger om anslutningen kan uppdateras i bakgrunden (asynkront). true om föredragen användning av anslutningen är att uppdatera asynkront i bakgrunden; false om föredragen användning av anslutningen är att uppdatera synkront i förgrunden.

```csharp
public bool BackgroundRefresh { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionPropertyBackgroundRefreshDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            try
            {
                // Åtkomst till den första externa anslutningen (förutsatt att en sådan finns)
                ExternalConnection connection = workbook.DataConnections[0];
                
                // Visa aktuellt BackgroundRefresh-värde
                Console.WriteLine("Initial BackgroundRefresh value: " + connection.BackgroundRefresh);
                
                // Växla BackgroundRefresh-värdet
                connection.BackgroundRefresh = !connection.BackgroundRefresh;
                Console.WriteLine("Updated BackgroundRefresh value: " + connection.BackgroundRefresh);
                
                // Spara arbetsboken med de ändrade anslutningsinställningarna
                workbook.Save("BackgroundRefreshDemo.xlsx");
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


