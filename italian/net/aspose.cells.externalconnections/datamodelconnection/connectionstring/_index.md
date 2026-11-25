---
title: "DataModelConnection.ConnectionString"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà DataModelConnection. La stringa di informazioni di connessione è usata per stabilire il contatto con una fonte dati OLE DB o ODBC"
type: docs
url: /it/net/aspose.cells.externalconnections/datamodelconnection/connectionstring/
---
## DataModelConnection.ConnectionString property

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
    using System.Runtime.Serialization;

    public class DataModelConnectionPropertyConnectionStringDemo
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

                // Visualizza il valore iniziale di ConnectionString (vuoto)
                Console.WriteLine("Initial ConnectionString: " + connection.ConnectionString);

                // Imposta la proprietà ConnectionString
                connection.ConnectionString = "Provider=SQLOLEDB;Data Source=Northwind;Integrated Security=SSPI";
                
                // Visualizza il valore aggiornato di ConnectionString
                Console.WriteLine("Updated ConnectionString: " + connection.ConnectionString);

                // Imposta le altre proprietà richieste per una connessione completa
                connection.Command = "SELECT * FROM Customers";
                connection.CommandType = OLEDBCommandType.SqlStatement;

                // Salva la cartella di lavoro con la connessione
                workbook.Save("ConnectionStringDemo.xlsx");
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


