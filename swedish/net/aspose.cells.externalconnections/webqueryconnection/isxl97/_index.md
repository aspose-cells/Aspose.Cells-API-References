---
title: "WebQueryConnection.IsXl97"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WebQueryConnection‑egenskap. Denna flagga finns för bakåtkompatibilitet med äldre befintliga kalkylbladsfiler och sätts till true om denna webbfråga skapades i Microsoft Excel 97. Detta är ett valfritt attribut som kan ignoreras"
type: docs
url: /sv/net/aspose.cells.externalconnections/webqueryconnection/isxl97/
---
## WebQueryConnection.IsXl97 property

Denna flagga finns för bakåtkompatibilitet med äldre befintliga kalkylbladsfiler, och sätts till true om denna webbfråga skapades i Microsoft Excel 97. Detta är ett valfritt attribut som kan ignoreras.

```csharp
public bool IsXl97 { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class WebQueryConnectionPropertyIsXl97Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            try
            {
                // Skapa ett kalkylblad med lite data för att göra exemplet meningsfullt
                Worksheet worksheet = workbook.Worksheets[0];
                worksheet.Cells["A1"].Value = "Sample Data";
                
                // Skapa en webbfrågeanslutning genom att läsa in från en befintlig fil eller skapa den på rätt sätt
                // Eftersom vi inte kan skapa WebQueryConnection direkt, kommer vi att åtkomma en befintlig
                if (workbook.DataConnections.Count > 0 && 
                    workbook.DataConnections[0] is WebQueryConnection connection)
                {
                    // Visa initialt IsXl97‑värde
                    Console.WriteLine("Initial IsXl97 value: " + connection.IsXl97);
                    
                    // Ställ in IsXl97 till true (eftersom den är läs‑skriv)
                    connection.IsXl97 = true;
                    Console.WriteLine("Updated IsXl97 value: " + connection.IsXl97);
                    
                    // Återställ IsXl97 till false
                    connection.IsXl97 = false;
                    Console.WriteLine("Final IsXl97 value: " + connection.IsXl97);
                    
                    // Spara arbetsboken
                    workbook.Save("WebQueryConnectionIsXl97Demo.xlsx");
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

* class [WebQueryConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


