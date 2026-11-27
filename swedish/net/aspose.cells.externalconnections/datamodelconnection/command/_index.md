---
title: "DataModelConnection.Command"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DataModelConnection‑egenskap. Strängen som innehåller databaskommandot som ska skickas till data provider API som kommer att interagera med den externa källan för att hämta data"
type: docs
url: /sv/net/aspose.cells.externalconnections/datamodelconnection/command/
---
## DataModelConnection.Command property

Strängen som innehåller databaskommandot att skicka till data‑leverantörens API som kommer att interagera med den externa källan för att hämta data

```csharp
public override string Command { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;
    using System.Runtime.Serialization;

    public class DataModelConnectionPropertyCommandDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            try
            {
                // Skapa en DataModelConnection‑instans med ett oinitierat objekt
                DataModelConnection connection = (DataModelConnection)FormatterServices.GetUninitializedObject(typeof(DataModelConnection));
                ((IList<ExternalConnection>)workbook.DataConnections).Add(connection);

                // Visa initialt Command‑värde (tomt)
                Console.WriteLine("Initial Command: " + connection.Command);

                // Ställ in Command‑egenskapen
                connection.Command = "SELECT * FROM Customers";
                
                // Visa det uppdaterade Command‑värdet
                Console.WriteLine("Updated Command: " + connection.Command);

                // Ställ in andra nödvändiga egenskaper för en fullständig anslutning
                connection.CommandType = OLEDBCommandType.SqlStatement;
                connection.ConnectionString = "Provider=SQLOLEDB;Data Source=Northwind;Integrated Security=SSPI";

                // Spara arbetsboken med anslutningen
                workbook.Save("CommandDemo.xlsx");
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

* class [DataModelConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


