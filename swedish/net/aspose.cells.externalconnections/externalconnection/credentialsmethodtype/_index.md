---
title: "ExternalConnection.CredentialsMethodType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ExternalConnection egenskap. Anger autentiseringsmetoden som ska användas när anslutningen etableras eller återupprättas"
type: docs
url: /sv/net/aspose.cells.externalconnections/externalconnection/credentialsmethodtype/
---
## ExternalConnection.CredentialsMethodType property

Anger autentiseringsmetoden som ska användas när anslutningen upprättas (eller återupprättas).

```csharp
public CredentialsMethodType CredentialsMethodType { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using Aspose.Cells.Pivot;
    using System;

    public class ExternalConnectionPropertyCredentialsMethodTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            try
            {
                // Lägg till ett kalkylblad och skapa en pivottabell för att etablera en extern anslutning
                Worksheet sheet = workbook.Worksheets[0];
                sheet.Cells["A1"].PutValue("Product");
                sheet.Cells["B1"].PutValue("Sales");
                sheet.Cells["A2"].PutValue("Apple");
                sheet.Cells["B2"].PutValue(1000);
                sheet.Cells["A3"].PutValue("Banana");
                sheet.Cells["B3"].PutValue(2000);

                // Skapa en pivottabell som kommer att ha en extern anslutning
                int index = sheet.PivotTables.Add("A1:B3", "C3", "PivotTable1");
                Aspose.Cells.Pivot.PivotTable pivotTable = sheet.PivotTables[index];

                // Hämta den externa anslutningen från pivottabellen
                ExternalConnection connection = pivotTable.GetSourceDataConnections()[0];

                // Visa det aktuella CredentialsMethodType-värdet
                Console.WriteLine("Initial CredentialsMethodType: " + connection.CredentialsMethodType);

                // Demonstrera att sätta egenskapen (eftersom den är läs-skriv)
                connection.CredentialsMethodType = CredentialsMethodType.Stored;
                Console.WriteLine("Updated CredentialsMethodType: " + connection.CredentialsMethodType);

                // Ange ett annat värde för att demonstrera
                connection.CredentialsMethodType = CredentialsMethodType.Integrated;
                Console.WriteLine("Changed CredentialsMethodType: " + connection.CredentialsMethodType);

                // Spara arbetsboken med de ändrade anslutningsinställningarna
                workbook.Save("CredentialsMethodTypeDemo.xlsx");
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

* enum [CredentialsMethodType](../../credentialsmethodtype/)
* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


