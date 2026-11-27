---
title: "ExternalConnection.ReconnectionMethod"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ExternalConnection egenskap. Anger vad kalkylprogrammet ska göra när en anslutning misslyckas. Standardvärdet är ReConnectionMethodType.Required"
type: docs
url: /sv/net/aspose.cells.externalconnections/externalconnection/reconnectionmethod/
---
## ExternalConnection.ReconnectionMethod property

Anger vad kalkylbladsapplikationen ska göra när en anslutning misslyckas. Standardvärdet är ReConnectionMethodType.Required.

```csharp
[Obsolete("Use ExternalConnection.ReconnectionMethodType property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public ReConnectionMethodType ReconnectionMethod { get; set; }
```

### Anmärkningar

OBS: Denna egenskap är nu föråldrad. Använd istället ExternalConnection.ReconnectionMethodType egenskap. Denna egenskap kommer att tas bort 12 månader senare från och med oktober 2017. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionPropertyReconnectionMethodDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            try
            {
                // Åtkomst till den första externa anslutningen (förutsatt att en sådan finns)
                ExternalConnection connection = workbook.DataConnections[0];
                
                // Visa det aktuella ReconnectionMethod-värdet (läsoperation)
                Console.WriteLine("Initial ReconnectionMethod value: " + connection.ReconnectionMethod);
                
                // Ange nya ReconnectionMethod-värden (eftersom den är läs-skriv)
                connection.ReconnectionMethod = ReConnectionMethodType.Always;
                Console.WriteLine("Updated ReconnectionMethod value: " + connection.ReconnectionMethod);
                
                connection.ReconnectionMethod = ReConnectionMethodType.Never;
                Console.WriteLine("Updated ReconnectionMethod value: " + connection.ReconnectionMethod);
                
                // Återställ till standardvärde
                connection.ReconnectionMethod = ReConnectionMethodType.Required;
                Console.WriteLine("Reset ReconnectionMethod value: " + connection.ReconnectionMethod);
                
                // Spara arbetsboken med de ändrade anslutningsinställningarna
                workbook.Save("ReconnectionMethodDemo.xlsx");
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


