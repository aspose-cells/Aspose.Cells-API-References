---
title: "ExternalConnection.ConnectionDescription"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ExternalConnection-egenskap. Anger användarbeskrivningen för denna anslutning"
type: docs
url: /sv/net/aspose.cells.externalconnections/externalconnection/connectiondescription/
---
## ExternalConnection.ConnectionDescription property

Anger användarbeskrivningen för denna anslutning

```csharp
public string ConnectionDescription { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using Aspose.Cells.Pivot;
    using System;

    public class ExternalConnectionPropertyConnectionDescriptionDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            try
            {
                // Lägg till ett kalkylblad med exempeldata
                Worksheet worksheet = workbook.Worksheets[0];
                worksheet.Cells["A1"].Value = "Product";
                worksheet.Cells["B1"].Value = "Sales";
                worksheet.Cells["A2"].Value = "Apple";
                worksheet.Cells["B2"].Value = 1000;
                worksheet.Cells["A3"].Value = "Banana";
                worksheet.Cells["B3"].Value = 2000;

                // Skapa en pivottabell för att etablera en extern anslutning
                int pivotIndex = worksheet.PivotTables.Add("A1:B3", "C3", "PivotTable1");
                Aspose.Cells.Pivot.PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

                // Hämta den externa anslutningen från pivottabellen
                ExternalConnection connection = pivotTable.GetSourceDataConnections()[0];

                // Visa det ursprungliga ConnectionDescription‑värdet
                Console.WriteLine("Initial ConnectionDescription: " + connection.ConnectionDescription);

                // Ange en ny beskrivning (eftersom den är läs‑skriv)
                connection.ConnectionDescription = "This connection retrieves sales data from internal sources";
                Console.WriteLine("Updated ConnectionDescription: " + connection.ConnectionDescription);

                // Rensa beskrivningen
                connection.ConnectionDescription = string.Empty;
                Console.WriteLine("Cleared ConnectionDescription: " + connection.ConnectionDescription);

                // Spara arbetsboken med den ändrade anslutningen
                workbook.Save("ConnectionDescriptionDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
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


