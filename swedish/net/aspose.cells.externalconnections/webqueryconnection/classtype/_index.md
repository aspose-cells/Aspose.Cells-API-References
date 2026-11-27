---
title: "WebQueryConnection.ClassType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WebQueryConnection egenskap. Hämtar typen av detta ExternalConnection-objekt"
type: docs
url: /sv/net/aspose.cells.externalconnections/webqueryconnection/classtype/
---
## WebQueryConnection.ClassType property

Hämtar typen av detta [`ExternalConnection`](../../externalconnection/)‑objekt.

```csharp
public override ExternalConnectionClassType ClassType { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class WebQueryConnectionPropertyClassTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            try
            {
                // Åtkomst till en befintlig webbfrågeanslutning eller skapa en via korrekt initiering
                if (workbook.DataConnections.Count > 0 && 
                    workbook.DataConnections[0] is WebQueryConnection connection)
                {
                    // Visa ClassType‑värdet (skrivskyddad egenskap).
                    Console.WriteLine("WebQueryConnection ClassType: " + connection.ClassType);
                    
                    // Verifiera det förväntade enum‑värdet för webbförfrågan
                    Console.WriteLine("Expected WebQuery enum value: " + 
                        (connection.ClassType == ExternalConnectionClassType.WebQuery ? "Match" : "Mismatch"));
                    
                    // Spara arbetsboken
                    workbook.Save("WebQueryConnectionClassTypeDemo.xlsx");
                }
                else
                {
                    Console.WriteLine("No web query connections found in the workbook.");
                }
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

* enum [ExternalConnectionClassType](../../externalconnectionclasstype/)
* class [WebQueryConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


