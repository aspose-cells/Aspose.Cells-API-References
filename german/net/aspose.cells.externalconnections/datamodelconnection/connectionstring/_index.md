---
title: "DataModelConnection.ConnectionString"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "DataModelConnection-Eigenschaft. Die Verbindungszeichenfolge wird verwendet, um Kontakt zu einer OLE DB- oder ODBC-Datenquelle herzustellen."
type: docs
url: /de/net/aspose.cells.externalconnections/datamodelconnection/connectionstring/
---
## DataModelConnection.ConnectionString property

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
    using System.Runtime.Serialization;

    public class DataModelConnectionPropertyConnectionStringDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            try
            {
                // Erstellen Sie eine DataModelConnection-Instanz mit einem nicht initialisierten Objekt
                DataModelConnection connection = (DataModelConnection)FormatterServices.GetUninitializedObject(typeof(DataModelConnection));
                ((IList<ExternalConnection>)workbook.DataConnections).Add(connection);

                // Initialen ConnectionString-Wert anzeigen (leer)
                Console.WriteLine("Initial ConnectionString: " + connection.ConnectionString);

                // Setze die ConnectionString-Eigenschaft
                connection.ConnectionString = "Provider=SQLOLEDB;Data Source=Northwind;Integrated Security=SSPI";
                
                // Zeigen Sie den aktualisierten ConnectionString-Wert an
                Console.WriteLine("Updated ConnectionString: " + connection.ConnectionString);

                // Setze weitere erforderliche Eigenschaften für eine vollständige Verbindung
                connection.Command = "SELECT * FROM Customers";
                connection.CommandType = OLEDBCommandType.SqlStatement;

                // Arbeitsmappe mit der Verbindung speichern
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

### Siehe auch

* class [DataModelConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


