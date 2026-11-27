---
title: "DBConnection.SecondCommand"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DBConnection egenskap. Specificerar en andra kommandotextsträng som sparas när PivotTable‑serverbaserade sidfält används. För ODBC‑anslutningar är serverCommand vanligtvis en bredare fråga än command; ingen WHERE‑klausul finns i den förra. Baserat på dessa två kommandon, Command och ServerCommand, kan parameter‑UI fyllas i och parametriserade frågor kan konstrueras."
type: docs
url: /sv/net/aspose.cells.externalconnections/dbconnection/secondcommand/
---
## DBConnection.SecondCommand property

Anger en andra kommandotextsträng som bevaras när PivotTable-serverbaserade sidfält används. För ODBC-anslutningar är serverCommand vanligtvis en bredare fråga än command (ingen WHERE-klausul finns i den förra). Baserat på dessa två kommandon (Command och ServerCommand) kan parameter‑UI fyllas i och parametriserade frågor konstrueras

```csharp
public override string SecondCommand { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class DBConnectionPropertySecondCommandDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            try
            {
                // Skapa en ny DBConnection‑instans genom att lägga till den i samlingen
                var connections = workbook.DataConnections;
                DBConnection dbConnection = (DBConnection)connections[0];
                
                // Skapa en grundläggande anslutning.
                dbConnection.ConnectionString = "Server=myServer;Database=myDB;";
                dbConnection.CommandType = OLEDBCommandType.SqlStatement;
                dbConnection.Command = "SELECT * FROM Customers WHERE Country = 'USA'";
                
                // Ange och demonstrera SecondCommand‑egenskapen.
                dbConnection.SecondCommand = "SELECT * FROM Customers";
                Console.WriteLine("SecondCommand value: " + dbConnection.SecondCommand);
                
                // Modifiera SecondCommand för att visa att den är skrivbar.
                dbConnection.SecondCommand = "SELECT * FROM Orders";
                Console.WriteLine("Updated SecondCommand value: " + dbConnection.SecondCommand);
                
                // Spara arbetsboken
                workbook.Save("SecondCommandDemo.xlsx");
                
                Console.WriteLine("SecondCommand demonstration completed successfully.");
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


