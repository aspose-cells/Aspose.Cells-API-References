---
title: "DBConnection.SecondCommand"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà DBConnection. Specifica una seconda stringa di testo del comando che viene mantenuta quando i campi pagina basati su server di PivotTable sono in uso. Per le connessioni ODBC serverCommand è solitamente una query più ampia rispetto a command, poiché nella prima non è presente la clausola WHERE. Sulla base di questi due comandi, Command e ServerCommand, l'interfaccia dei parametri può essere popolata e possono essere costruite query parametrizzate"
type: docs
url: /it/net/aspose.cells.externalconnections/dbconnection/secondcommand/
---
## DBConnection.SecondCommand property

Specifica una seconda stringa di testo del comando che viene mantenuta quando i campi di pagina basati su server della PivotTable sono in uso. Per le connessioni ODBC, serverCommand è solitamente una query più ampia rispetto a command (no WHERE clause is present in the former). Based on these 2 commands(Command and ServerCommand), parameter UI can be populated and parameterized queries can be constructed

```csharp
public override string SecondCommand { get; set; }
```

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            try
            {
                // Crea una nuova istanza DBConnection aggiungendola alla collezione
                var connections = workbook.DataConnections;
                DBConnection dbConnection = (DBConnection)connections[0];
                
                // Configura una connessione di base
                dbConnection.ConnectionString = "Server=myServer;Database=myDB;";
                dbConnection.CommandType = OLEDBCommandType.SqlStatement;
                dbConnection.Command = "SELECT * FROM Customers WHERE Country = 'USA'";
                
                // Imposta e dimostra la proprietà SecondCommand
                dbConnection.SecondCommand = "SELECT * FROM Customers";
                Console.WriteLine("SecondCommand value: " + dbConnection.SecondCommand);
                
                // Modifica il SecondCommand per mostrare che è scrivibile
                dbConnection.SecondCommand = "SELECT * FROM Orders";
                Console.WriteLine("Updated SecondCommand value: " + dbConnection.SecondCommand);
                
                // Salva la cartella di lavoro
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

### Vedi anche

* class [DBConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


