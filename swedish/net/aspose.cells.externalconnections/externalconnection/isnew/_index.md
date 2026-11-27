---
title: "ExternalConnection.IsNew"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ExternalConnection egenskap. True om kopplingen inte har uppdaterats för första gången annars false. Detta tillstånd kan uppstå när användaren sparar filen innan en fråga har slutförts"
type: docs
url: /sv/net/aspose.cells.externalconnections/externalconnection/isnew/
---
## ExternalConnection.IsNew property

True om anslutningen inte har uppdaterats för första gången; annars false. Detta tillstånd kan uppstå när användaren sparar filen innan en fråga har slutförts.

```csharp
public bool IsNew { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionPropertyIsNewDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            try
            {
                // Åtkomst till den första externa anslutningen (nyss skapade anslutningar är vanligtvis "IsNew")
                ExternalConnection connection = workbook.DataConnections[0];
                
                // Visa det ursprungliga IsNew‑värdet
                Console.WriteLine("Initial IsNew value: " + connection.IsNew);
                
                // Eftersom IsNew är läs‑skriv, demonstrera hur man sätter den
                connection.IsNew = false;
                Console.WriteLine("Updated IsNew value: " + connection.IsNew);
                
                // Spara arbetsboken med de ändrade anslutningsinställningarna
                workbook.Save("IsNewDemo.xlsx");
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


