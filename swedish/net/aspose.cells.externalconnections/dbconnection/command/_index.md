---
title: "DBConnection.Command"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DBConnection‑egenskap. Strängen som innehåller databas‑kommandot som ska skickas till data‑leverantörens API som kommer att interagera med den externa källan för att hämta data"
type: docs
url: /sv/net/aspose.cells.externalconnections/dbconnection/command/
---
## DBConnection.Command property

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

    public class DBConnectionPropertyCommandDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            try
            {
                // Åtkomst till samlingen av externa anslutningar.
                ExternalConnectionCollection connections = workbook.DataConnections;

                // Hitta den första DBConnection i samlingen (om någon).
                DBConnection dbConn = null;
                foreach (ExternalConnection conn in connections)
                {
                    if (conn is DBConnection dbConnection)
                    {
                        dbConn = dbConnection;
                        break;
                    }
                }

                if (dbConn == null)
                {
                    Console.WriteLine("No DBConnection objects found in the workbook.");
                }
                else
                {
                    // Visa det aktuella Command‑värdet (läsoperation)
                    Console.WriteLine("Current Command: " + dbConn.Command);

                    // Demonstrera att sätta Command (läslig‑skrivbar egenskap)
                    dbConn.Command = "SELECT * FROM Customers";
                    Console.WriteLine("Updated Command: " + dbConn.Command);
                }

                // Spara arbetsboken
                workbook.Save("CommandDemo.xlsx");
                Console.WriteLine("Workbook saved as CommandDemo.xlsx");
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

* class [DBConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


