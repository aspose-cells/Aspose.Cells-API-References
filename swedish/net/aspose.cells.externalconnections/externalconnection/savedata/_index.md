---
title: "ExternalConnection.SaveData"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ExternalConnection-egenskap. Sant om den externa data som hämtas via anslutningen för att fylla en tabell ska sparas med arbetsboken, annars falskt"
type: docs
url: /sv/net/aspose.cells.externalconnections/externalconnection/savedata/
---
## ExternalConnection.SaveData property

True om den externa data som hämtas via anslutningen för att fylla i en tabell ska sparas med arbetsboken; annars false.

```csharp
public bool SaveData { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionPropertySaveDataDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            try
            {
                // Åtkomst till den första externa anslutningen (förutsatt att en sådan finns)
                ExternalConnection connection = workbook.DataConnections[0];
                
                // Visa det aktuella SaveData‑värdet
                Console.WriteLine("Initial SaveData value: " + connection.SaveData);
                
                // Demonstrera att sätta egenskapen (eftersom den är läs-skriv)
                connection.SaveData = !connection.SaveData;
                Console.WriteLine("Updated SaveData value: " + connection.SaveData);
                
                // Spara arbetsboken med de ändrade anslutningsinställningarna
                workbook.Save("SaveDataDemo.xlsx");
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


