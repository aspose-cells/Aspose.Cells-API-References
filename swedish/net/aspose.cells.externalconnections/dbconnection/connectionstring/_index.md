---
title: "DBConnection.ConnectionString"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DBConnection‑egenskap. Strängen med anslutningsinformation används för att kontakta en OLE DB‑ eller ODBC‑datakälla"
type: docs
url: /sv/net/aspose.cells.externalconnections/dbconnection/connectionstring/
---
## DBConnection.ConnectionString property

Anslutningsinformationssträngen används för att kontakta en OLE DB‑ eller ODBC‑datakälla.

```csharp
public override string ConnectionString { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class DBConnectionPropertyConnectionStringDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            try
            {
                // Åtkomst till samlingen av externa anslutningar.
                ExternalConnectionCollection connections = workbook.DataConnections;

                // Skapa en ny DBConnection genom att lägga till den i samlingen
                DBConnection dbConnection = (DBConnection)connections[connections.Count];

                // Visa det ursprungliga ConnectionString‑värdet
                Console.WriteLine("Initial ConnectionString: " + dbConnection.ConnectionString);

                // Ange en ny anslutningssträng
                dbConnection.ConnectionString = "Provider=Microsoft.Jet.OLEDB.4.0;Data Source=C:\\data\\database.mdb;";

                // Visa det uppdaterade ConnectionString‑värdet
                Console.WriteLine("Updated ConnectionString: " + dbConnection.ConnectionString);

                // Spara arbetsboken
                workbook.Save("ConnectionStringDemo.xlsx");
                Console.WriteLine("ConnectionString demonstration completed successfully.");
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


