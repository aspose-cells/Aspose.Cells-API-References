---
title: "DataModelConnection.Command"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "DataModelConnection proprietà. La stringa contenente il comando del database da passare all'API del provider di dati che interagirà con la fonte esterna per recuperare i dati"
type: docs
url: /it/net/aspose.cells.externalconnections/datamodelconnection/command/
---
## DataModelConnection.Command property

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
    using System.Runtime.Serialization;

    public class DataModelConnectionPropertyCommandDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            try
            {
                // Crea un'istanza di DataModelConnection utilizzando un oggetto non inizializzato
                DataModelConnection connection = (DataModelConnection)FormatterServices.GetUninitializedObject(typeof(DataModelConnection));
                ((IList<ExternalConnection>)workbook.DataConnections).Add(connection);

                // Visualizza il valore iniziale di Command (vuoto)
                Console.WriteLine("Initial Command: " + connection.Command);

                // Imposta la proprietà Command
                connection.Command = "SELECT * FROM Customers";
                
                // Visualizza il valore aggiornato di Command
                Console.WriteLine("Updated Command: " + connection.Command);

                // Imposta le altre proprietà richieste per una connessione completa
                connection.CommandType = OLEDBCommandType.SqlStatement;
                connection.ConnectionString = "Provider=SQLOLEDB;Data Source=Northwind;Integrated Security=SSPI";

                // Salva la cartella di lavoro con la connessione
                workbook.Save("CommandDemo.xlsx");
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

* class [DataModelConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


