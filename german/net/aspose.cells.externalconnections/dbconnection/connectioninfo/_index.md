---
title: "DBConnection.ConnectionInfo"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "DBConnection‑Eigenschaft. Der Verbindungszeichenfolgen‑String wird verwendet, um Kontakt zu einer OLE DB- oder ODBC-Datenquelle herzustellen"
type: docs
url: /de/net/aspose.cells.externalconnections/dbconnection/connectioninfo/
---
## DBConnection.ConnectionInfo property

Die Verbindungsinformationszeichenkette wird verwendet, um Kontakt mit einer OLE DB- oder ODBC-Datenquelle aufzunehmen.

```csharp
[Obsolete("Use ExternalConnection.ConnectionString property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public string ConnectionInfo { get; set; }
```

### Hinweise

HINWEIS: Diese Eigenschaft ist jetzt veraltet. Verwenden Sie stattdessen die Eigenschaft ExternalConnection.ConnectionString. Diese Methode wird 12 Monate später, seit Oktober 2024, entfernt werden. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            try
            {
                // Erstelle eine neue DBConnection‑Instanz, indem du sie zur Sammlung hinzufügst
                var connections = workbook.DataConnections;
                DBConnection dbConnection = (DBConnection)connections[connections.Count];

                // Richten Sie eine einfache Verbindung ein, um die ConnectionInfo-Eigenschaft zu demonstrieren
                dbConnection.ConnectionString = "Provider=Microsoft.Jet.OLEDB.4.0;Data Source=C:\\data\\database.mdb;";
                dbConnection.CommandType = OLEDBCommandType.TableName;
                dbConnection.Command = "Customers";

                // Zeigen Sie den aktuellen Wert der ConnectionInfo-Eigenschaft an
                Console.WriteLine("Current ConnectionInfo value: " + dbConnection.ConnectionInfo);

                // Da ConnectionInfo nicht schreibgeschützt ist, demonstrieren Sie das Setzen
                dbConnection.ConnectionInfo = "Provider=Microsoft.Jet.OLEDB.4.0;Data Source=D:\\data\\database.mdb;";
                Console.WriteLine("Updated ConnectionInfo value: " + dbConnection.ConnectionInfo);

                // Speichere die Arbeitsmappe
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

### Siehe auch

* class [DBConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


