---
title: "DBConnection.ConnectionString"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà DBConnection. La stringa di informazioni di connessione è usata per stabilire un collegamento con una fonte dati OLE DB o ODBC"
type: docs
url: /it/net/aspose.cells.externalconnections/dbconnection/connectionstring/
---
## DBConnection.ConnectionString property

La stringa di informazioni della connessione è usata per contattare una fonte dati OLE DB o ODBC.

```csharp
public override string ConnectionString { get; set; }
```

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            try
            {
                // Accedi alla raccolta di connessioni esterne
                ExternalConnectionCollection connections = workbook.DataConnections;

                // Crea un nuovo DBConnection aggiungendolo alla collezione
                DBConnection dbConnection = (DBConnection)connections[connections.Count];

                // Visualizza il valore iniziale di ConnectionString
                Console.WriteLine("Initial ConnectionString: " + dbConnection.ConnectionString);

                // Imposta una nuova stringa di connessione
                dbConnection.ConnectionString = "Provider=Microsoft.Jet.OLEDB.4.0;Data Source=C:\\data\\database.mdb;";

                // Visualizza il valore aggiornato di ConnectionString
                Console.WriteLine("Updated ConnectionString: " + dbConnection.ConnectionString);

                // Salva la cartella di lavoro
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

### Vedi anche

* class [DBConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


