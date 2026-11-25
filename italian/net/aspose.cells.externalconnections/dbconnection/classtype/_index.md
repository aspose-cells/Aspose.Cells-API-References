---
title: "DBConnection.ClassType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà DBConnection. Restituisce il tipo di questo oggetto ExternalConnection"
type: docs
url: /it/net/aspose.cells.externalconnections/dbconnection/classtype/
---
## DBConnection.ClassType property

Ottiene il tipo di questo [`ExternalConnection`](../../externalconnection/) oggetto.

```csharp
public override ExternalConnectionClassType ClassType { get; }
```

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            try
            {
                // Crea una nuova istanza DBConnection aggiungendola alla collezione
                // Poiché DBConnection non ha un costruttore pubblico senza parametri,
                // lasceremo che la collezione lo crei per noi
                var connections = workbook.DataConnections;
                DBConnection dbConnection = (DBConnection)connections[connections.Count];
                
                // Visualizza il valore di ClassType (proprietà di sola lettura)
                Console.WriteLine("DBConnection ClassType: " + dbConnection.ClassType);
                
                // Dimostra l'impostazione di altre proprietà per rendere l'esempio più significativo
                dbConnection.ConnectionString = "Server=myServerAddress;Database=myDataBase;";
                dbConnection.CommandType = OLEDBCommandType.TableName;
                dbConnection.Command = "Customers";
                
                // Salva la cartella di lavoro
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

### Vedi anche

* enum [ExternalConnectionClassType](../../externalconnectionclasstype/)
* class [DBConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


