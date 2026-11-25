---
title: "DBConnection.Command"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà DBConnection. La stringa contenente il comando del database da passare all'API del provider di dati che interagirà con la fonte esterna per recuperare i dati"
type: docs
url: /it/net/aspose.cells.externalconnections/dbconnection/command/
---
## DBConnection.Command property

La stringa contenente il comando del database da passare all'API del provider dati che interagirà con la fonte esterna per recuperare i dati

```csharp
public override string Command { get; set; }
```

### Esempi

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
            // Crea un nuovo workbook
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
                    // Visualizza il valore corrente di Command (operazione di lettura)
                    Console.WriteLine("Current Command: " + dbConn.Command);

                    // Dimostra l'impostazione di Command (proprietà di lettura‑scrittura)
                    dbConn.Command = "SELECT * FROM Customers";
                    Console.WriteLine("Updated Command: " + dbConn.Command);
                }

                // Salva la cartella di lavoro
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

### Vedi anche

* class [DBConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


