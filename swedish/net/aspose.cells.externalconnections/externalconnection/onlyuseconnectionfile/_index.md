---
title: "ExternalConnection.OnlyUseConnectionFile"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ExternalConnection-egenskap. Anger om kalkylprogrammet alltid och endast ska använda anslutningsinformationen i den externa anslutningsfilen som anges av odcFile-attributet när anslutningen uppdateras. Om falskt ska kalkylprogrammet följa proceduren som anges av reconnectionMethod-attributet"
type: docs
url: /sv/net/aspose.cells.externalconnections/externalconnection/onlyuseconnectionfile/
---
## ExternalConnection.OnlyUseConnectionFile property

Indikerar om kalkylbladsapplikationen alltid och endast ska använda anslutningsinformationen i den externa anslutningsfilen som anges av odcFile‑attributet när anslutningen uppdateras. Om false ska kalkylbladsapplikationen följa proceduren som anges av reconnectionMethod‑attributet.

```csharp
public bool OnlyUseConnectionFile { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionPropertyOnlyUseConnectionFileDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            try
            {
                // Åtkomst till den första externa anslutningen (förutsatt att en sådan finns)
                ExternalConnection connection = workbook.DataConnections[0];
                
                // Visa det aktuella OnlyUseConnectionFile-värdet
                Console.WriteLine("Initial OnlyUseConnectionFile value: " + connection.OnlyUseConnectionFile);
                
                // Ange ett nytt OnlyUseConnectionFile-värde (eftersom det är läs‑skriv)
                connection.OnlyUseConnectionFile = true;
                Console.WriteLine("Updated OnlyUseConnectionFile value: " + connection.OnlyUseConnectionFile);
                
                // Växla värdet för att demonstrera inställningsmöjlighet
                connection.OnlyUseConnectionFile = !connection.OnlyUseConnectionFile;
                Console.WriteLine("Toggled OnlyUseConnectionFile value: " + connection.OnlyUseConnectionFile);
                
                // Spara arbetsboken med de ändrade anslutningsinställningarna
                workbook.Save("OnlyUseConnectionFileDemo.xlsx");
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


