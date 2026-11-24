---
title: "DBConnection.ConnectionString"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "DBConnection‑Eigenschaft. Der Verbindungszeichenfolgen‑String wird verwendet, um Kontakt zu einer OLE DB- oder ODBC-Datenquelle herzustellen"
type: docs
url: /de/net/aspose.cells.externalconnections/dbconnection/connectionstring/
---
## DBConnection.ConnectionString property

Die Verbindungsinformationszeichenkette wird verwendet, um Kontakt mit einer OLE DB- oder ODBC-Datenquelle aufzunehmen.

```csharp
public override string ConnectionString { get; set; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            try
            {
                // Zugriff auf die Sammlung externer Verbindungen
                ExternalConnectionCollection connections = workbook.DataConnections;

                // Erstellen Sie eine neue DBConnection, indem Sie sie zur Sammlung hinzufügen
                DBConnection dbConnection = (DBConnection)connections[connections.Count];

                // Zeigen Sie den anfänglichen ConnectionString-Wert an
                Console.WriteLine("Initial ConnectionString: " + dbConnection.ConnectionString);

                // Legen Sie einen neuen ConnectionString fest
                dbConnection.ConnectionString = "Provider=Microsoft.Jet.OLEDB.4.0;Data Source=C:\\data\\database.mdb;";

                // Zeigen Sie den aktualisierten ConnectionString-Wert an
                Console.WriteLine("Updated ConnectionString: " + dbConnection.ConnectionString);

                // Speichere die Arbeitsmappe
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

### Siehe auch

* class [DBConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


