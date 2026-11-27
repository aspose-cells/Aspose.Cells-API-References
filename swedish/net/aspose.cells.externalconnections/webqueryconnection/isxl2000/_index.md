---
title: "WebQueryConnection.IsXl2000"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WebQueryConnection‑egenskap. Denna flagga finns för bakåtkompatibilitet med äldre befintliga kalkylbladsfiler och sätts till true om denna webbfråga uppdaterades i ett kalkylbladsprogram som är nyare än eller lika med Microsoft Excel 2000. Detta är ett valfritt attribut som kan ignoreras"
type: docs
url: /sv/net/aspose.cells.externalconnections/webqueryconnection/isxl2000/
---
## WebQueryConnection.IsXl2000 property

Denna flagga finns för bakåtkompatibilitet med äldre befintliga kalkylbladsfiler, och sätts till true om denna webbfråga uppdaterades i ett kalkylbladsprogram nyare än eller lika med Microsoft Excel 2000. Detta är ett valfritt attribut som kan ignoreras.

```csharp
public bool IsXl2000 { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class WebQueryConnectionPropertyIsXl2000Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            try
            {
                // Åtkomst till den första befintliga webbfrågeanslutningen (om någon)
                if (workbook.DataConnections.Count > 0 && 
                    workbook.DataConnections[0] is WebQueryConnection connection)
                {
                    // Visa initialt IsXl2000‑värde
                    Console.WriteLine("Initial IsXl2000 value: " + connection.IsXl2000);

                    // Ställ in IsXl2000 till true (eftersom den är läs‑skriv)
                    connection.IsXl2000 = true;
                    Console.WriteLine("Updated IsXl2000 value: " + connection.IsXl2000);

                    // Ställ in IsXl2000 tillbaka till false
                    connection.IsXl2000 = false;
                    Console.WriteLine("Final IsXl2000 value: " + connection.IsXl2000);

                    // Spara arbetsboken
                    workbook.Save("WebQueryConnectionIsXl2000Demo.xlsx");
                }
                else
                {
                    Console.WriteLine("No web query connection found in the workbook.");
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


