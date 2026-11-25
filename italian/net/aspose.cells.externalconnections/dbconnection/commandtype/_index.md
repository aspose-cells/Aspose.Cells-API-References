---
title: "DBConnection.CommandType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà DBConnection. Specifica il tipo di comando OLE DB. 1. Query specifica il nome di un cubo 2. Query specifica un'istruzione SQL 3. Query specifica il nome di una tabella 4. Query specifica che sono state fornite informazioni predefinite ed è compito del provider interpretarle. 5. Query è contro un List Data Provider basato sul web"
type: docs
url: /it/net/aspose.cells.externalconnections/dbconnection/commandtype/
---
## DBConnection.CommandType property

Specifica il tipo di comando OLE DB. 1. La query specifica un nome di cubo 2. La query specifica un'istruzione SQL 3. La query specifica un nome di tabella 4. La query specifica che sono state fornite informazioni predefinite, e spetta al provider interpretarle. 5. La query è rivolta a un provider di dati elenco basato sul web.

```csharp
public override OLEDBCommandType CommandType { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using System;
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;

    public class DBConnectionPropertyCommandTypeDemo
    {
        public static void Run()
        {
            // Inizializza una cartella di lavoro (vuota o da un file che può contenere connessioni)
            Workbook workbook = new Workbook();

            try
            {
                // Accedi alla raccolta di connessioni esterne
                ExternalConnectionCollection connections = workbook.DataConnections;

                // Trova il primo DBConnection nella raccolta (se presente)
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
                    // Visualizza il valore corrente di CommandType
                    Console.WriteLine("Original CommandType: " + dbConn.CommandType);

                    // Dimostra l'impostazione di CommandType (proprietà di lettura‑scrittura)
                    dbConn.CommandType = OLEDBCommandType.SqlStatement;
                    Console.WriteLine("Updated CommandType: " + dbConn.CommandType);
                }

                // Salva la cartella di lavoro (anche se non modificata) per illustrare un flusso completo
                workbook.Save("CommandTypeDemo.xlsx");
                Console.WriteLine("Workbook saved as CommandTypeDemo.xlsx");
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

* enum [OLEDBCommandType](../../oledbcommandtype/)
* class [DBConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


