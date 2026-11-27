---
title: "DBConnection.ClassType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DBConnection egenskap. Hämtar typen av detta ExternalConnection‑objekt."
type: docs
url: /sv/net/aspose.cells.externalconnections/dbconnection/classtype/
---
## DBConnection.ClassType property

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

    public class DBConnectionPropertyClassTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            try
            {
                // Skapa en ny DBConnection‑instans genom att lägga till den i samlingen
                // Eftersom DBConnection inte har en publik parameterlös konstruktor,
                // låter vi samlingen skapa den åt oss.
                var connections = workbook.DataConnections;
                DBConnection dbConnection = (DBConnection)connections[connections.Count];
                
                // Visa ClassType‑värdet (skrivskyddad egenskap).
                Console.WriteLine("DBConnection ClassType: " + dbConnection.ClassType);
                
                // Demonstrera att sätta andra egenskaper för att göra exemplet mer meningsfullt
                dbConnection.ConnectionString = "Server=myServerAddress;Database=myDataBase;";
                dbConnection.CommandType = OLEDBCommandType.TableName;
                dbConnection.Command = "Customers";
                
                // Spara arbetsboken
                workbook.Save("DBConnectionDemo.xlsx");
                
                Console.WriteLine("ClassType demonstration completed successfully.");
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
* class [DBConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


