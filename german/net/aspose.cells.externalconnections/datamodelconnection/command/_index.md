---
title: "DataModelConnection.Command"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "DataModelConnection-Eigenschaft. Die Zeichenkette, die den Datenbankbefehl enthält, der an die API des Datenproviders übergeben wird, um mit der externen Quelle zu interagieren und Daten abzurufen."
type: docs
url: /de/net/aspose.cells.externalconnections/datamodelconnection/command/
---
## DataModelConnection.Command property

Die Zeichenkette, die den Datenbankbefehl enthält, der an die API des Datenanbieters übergeben wird, um mit der externen Quelle zu interagieren und Daten abzurufen

```csharp
public override string Command { get; set; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            try
            {
                // Erstellen Sie eine DataModelConnection-Instanz mit einem nicht initialisierten Objekt
                DataModelConnection connection = (DataModelConnection)FormatterServices.GetUninitializedObject(typeof(DataModelConnection));
                ((IList<ExternalConnection>)workbook.DataConnections).Add(connection);

                // Initialen Command-Wert anzeigen (leer)
                Console.WriteLine("Initial Command: " + connection.Command);

                // Setze die Command-Eigenschaft
                connection.Command = "SELECT * FROM Customers";
                
                // Aktualisierten Command-Wert anzeigen
                Console.WriteLine("Updated Command: " + connection.Command);

                // Setze weitere erforderliche Eigenschaften für eine vollständige Verbindung
                connection.CommandType = OLEDBCommandType.SqlStatement;
                connection.ConnectionString = "Provider=SQLOLEDB;Data Source=Northwind;Integrated Security=SSPI";

                // Arbeitsmappe mit der Verbindung speichern
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

### Siehe auch

* class [DataModelConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


