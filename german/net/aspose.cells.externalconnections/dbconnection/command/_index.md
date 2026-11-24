---
title: "DBConnection.Command"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "DBConnection-Eigenschaft. Die Zeichenkette, die den Datenbankbefehl enthält, der an die API des Datenanbieters übergeben wird, um mit der externen Quelle zu interagieren und Daten abzurufen"
type: docs
url: /de/net/aspose.cells.externalconnections/dbconnection/command/
---
## DBConnection.Command property

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

    public class DBConnectionPropertyCommandDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            try
            {
                // Zugriff auf die Sammlung externer Verbindungen
                ExternalConnectionCollection connections = workbook.DataConnections;

                // Finde die erste DBConnection in der Sammlung (falls vorhanden)
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
                    // Zeigen Sie den aktuellen Command-Wert an (Lesevorgang)
                    Console.WriteLine("Current Command: " + dbConn.Command);

                    // Demonstrieren Sie das Setzen von Command (Lese‑/Schreib‑Eigenschaft)
                    dbConn.Command = "SELECT * FROM Customers";
                    Console.WriteLine("Updated Command: " + dbConn.Command);
                }

                // Speichere die Arbeitsmappe
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

### Siehe auch

* class [DBConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


