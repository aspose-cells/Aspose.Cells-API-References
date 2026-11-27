---
title: "ExternalConnection.ReconnectionMethodType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ExternalConnection egenskap. Anger vad kalkylprogrammet ska göra när en anslutning misslyckas. Standardvärdet är ReConnectionMethodType.Required"
type: docs
url: /sv/net/aspose.cells.externalconnections/externalconnection/reconnectionmethodtype/
---
## ExternalConnection.ReconnectionMethodType property

Anger vad kalkylbladsapplikationen ska göra när en anslutning misslyckas. Standardvärdet är ReConnectionMethodType.Required.

```csharp
public ReConnectionMethodType ReconnectionMethodType { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionPropertyReconnectionMethodTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            try
            {
                // Åtkomst till den första externa anslutningen (förutsatt att en sådan finns)
                ExternalConnection connection = workbook.DataConnections[0];
                
                // Visa det aktuella ReconnectionMethodType‑värdet
                Console.WriteLine("Initial ReconnectionMethodType: " + connection.ReconnectionMethodType);
                
                // Demonstrera att sätta egenskapen (eftersom den är läs-skriv)
                connection.ReconnectionMethodType = ReConnectionMethodType.Always;
                Console.WriteLine("Updated ReconnectionMethodType: " + connection.ReconnectionMethodType);
                
                // Cykla igenom möjliga värden för att demonstrera inställningsmöjligheten
                foreach (ReConnectionMethodType method in Enum.GetValues(typeof(ReConnectionMethodType)))
                {
                    connection.ReconnectionMethodType = method;
                    Console.WriteLine($"ReconnectionMethodType set to: {method}");
                }
                
                // Spara arbetsboken med de ändrade anslutningsinställningarna
                workbook.Save("ReconnectionMethodTypeDemo.xlsx");
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

* enum [ReConnectionMethodType](../../reconnectionmethodtype/)
* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


