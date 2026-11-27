---
title: "ExternalConnection.RefreshInternal"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ExternalConnection egenskap. Anger antalet minuter mellan automatiska uppdateringar av anslutningen"
type: docs
url: /sv/net/aspose.cells.externalconnections/externalconnection/refreshinternal/
---
## ExternalConnection.RefreshInternal property

Anger antalet minuter mellan automatiska uppdateringar av anslutningen.

```csharp
public int RefreshInternal { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionPropertyRefreshInternalDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata för att göra exemplet meningsfullt
            worksheet.Cells["A1"].Value = "Connection Demo";
            
            try
            {
                // Skapa en datakoppling (med hjälp av basklassen ExternalConnection)
                ExternalConnection connection = workbook.DataConnections[0];
                
                // Ställ in och visa egenskapen RefreshInternal
                connection.RefreshInternal = 30; // Refresh every 30 minutes
                Console.WriteLine("RefreshInternal value: " + connection.RefreshInternal);
                
                // Ändra uppdateringsintervallet
                connection.RefreshInternal = 60;
                Console.WriteLine("Updated RefreshInternal value: " + connection.RefreshInternal);
                
                // Spara arbetsboken med anslutningsinställningarna
                workbook.Save("RefreshInternalDemo.xlsx");
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


