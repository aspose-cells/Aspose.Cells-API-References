---
title: "DBConnection.ConnectionInfo"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà DBConnection. La stringa di informazioni di connessione è usata per stabilire un collegamento con una fonte dati OLE DB o ODBC"
type: docs
url: /it/net/aspose.cells.externalconnections/dbconnection/connectioninfo/
---
## DBConnection.ConnectionInfo property

La stringa di informazioni della connessione è usata per contattare una fonte dati OLE DB o ODBC.

```csharp
[Obsolete("Use ExternalConnection.ConnectionString property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public string ConnectionInfo { get; set; }
```

### Osservazioni

NOTA: Questa proprietà è ora obsoleta. Invece, si prega di utilizzare la proprietà ExternalConnection.ConnectionString. Questo metodo sarà rimosso tra 12 mesi a partire da ottobre 2024. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class DBConnectionPropertyConnectionInfoDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            try
            {
                // Crea una nuova istanza DBConnection aggiungendola alla collezione
                var connections = workbook.DataConnections;
                DBConnection dbConnection = (DBConnection)connections[connections.Count];

                // Configura una connessione di base per dimostrare la proprietà ConnectionInfo
                dbConnection.ConnectionString = "Provider=Microsoft.Jet.OLEDB.4.0;Data Source=C:\\data\\database.mdb;";
                dbConnection.CommandType = OLEDBCommandType.TableName;
                dbConnection.Command = "Customers";

                // Visualizza il valore corrente della proprietà ConnectionInfo
                Console.WriteLine("Current ConnectionInfo value: " + dbConnection.ConnectionInfo);

                // Poiché ConnectionInfo non è di sola lettura, dimostra l'impostazione
                dbConnection.ConnectionInfo = "Provider=Microsoft.Jet.OLEDB.4.0;Data Source=D:\\data\\database.mdb;";
                Console.WriteLine("Updated ConnectionInfo value: " + dbConnection.ConnectionInfo);

                // Salva la cartella di lavoro
                workbook.Save("ConnectionInfoDemo.xlsx");

                Console.WriteLine("ConnectionInfo demonstration completed successfully.");
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


