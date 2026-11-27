---
title: "ExternalConnection.OdcFile"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ExternalConnection-egenskap. Anger den fullständiga sökvägen till den externa anslutningsfilen som denna anslutning skapades från. Om en anslutning misslyckas under ett försök att uppdatera data och reconnectionMethod1, kommer kalkylbladsprogrammet att försöka igen med information från den externa anslutningsfilen istället för anslutningsobjektet som är inbäddat i arbetsboken"
type: docs
url: /sv/net/aspose.cells.externalconnections/externalconnection/odcfile/
---
## ExternalConnection.OdcFile property

Anger den fullständiga sökvägen till den externa anslutningsfilen som denna anslutning skapades från. Om en anslutning misslyckas under ett försök att uppdatera data, och reconnectionMethod=1, kommer kalkylbladsapplikationen att försöka igen med information från den externa anslutningsfilen istället för anslutningsobjektet som är inbäddat i arbetsboken.

```csharp
public string OdcFile { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionPropertyOdcFileDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            try
            {
                // Åtkomst till den första externa anslutningen (förutsatt att en sådan finns)
                ExternalConnection connection = workbook.DataConnections[0];
                
                // Visa aktuellt OdcFile-värde
                Console.WriteLine("Initial OdcFile value: " + connection.OdcFile);
                
                // Ange ett nytt OdcFile-värde (eftersom det är läs-skriv)
                connection.OdcFile = @"C:\Connections\ExternalData.odc";
                Console.WriteLine("Updated OdcFile value: " + connection.OdcFile);
                
                // Rensa OdcFile-värdet
                connection.OdcFile = string.Empty;
                Console.WriteLine("Cleared OdcFile value: " + connection.OdcFile);
                
                // Spara arbetsboken med de ändrade anslutningsinställningarna
                workbook.Save("OdcFileDemo.xlsx");
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


