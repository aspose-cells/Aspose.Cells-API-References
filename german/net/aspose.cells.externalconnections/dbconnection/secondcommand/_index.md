---
title: "DBConnection.SecondCommand"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "DBConnection-Eigenschaft. Gibt einen zweiten Befehls‑Textstring an, der beibehalten wird, wenn serverbasierte PivotTable‑Seitenfelder verwendet werden. Für ODBC‑Verbindungen ist serverCommand normalerweise eine umfassendere Abfrage als command, da im Ersteren keine WHERE‑Klausel vorhanden ist. Auf Basis dieser beiden Befehle, Command und ServerCommand, kann die Parameter‑UI gefüllt und parametrisierte Abfragen erstellt werden."
type: docs
url: /de/net/aspose.cells.externalconnections/dbconnection/secondcommand/
---
## DBConnection.SecondCommand property

Gibt eine zweite Befehlszeichenfolge an, die gespeichert wird, wenn serverbasierte Seitenfelder einer PivotTable verwendet werden. Für ODBC-Verbindungen ist serverCommand in der Regel eine umfangreichere Abfrage als command (es ist keine WHERE‑Klausel in ersterer enthalten). Basierend auf diesen beiden Befehlen (Command und ServerCommand) kann die Parameter‑UI gefüllt und parametrisierte Abfragen erstellt werden

```csharp
public override string SecondCommand { get; set; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            try
            {
                // Erstelle eine neue DBConnection‑Instanz, indem du sie zur Sammlung hinzufügst
                var connections = workbook.DataConnections;
                DBConnection dbConnection = (DBConnection)connections[0];
                
                // Richten Sie eine einfache Verbindung ein
                dbConnection.ConnectionString = "Server=myServer;Database=myDB;";
                dbConnection.CommandType = OLEDBCommandType.SqlStatement;
                dbConnection.Command = "SELECT * FROM Customers WHERE Country = 'USA'";
                
                // Setzen und demonstrieren Sie die SecondCommand‑Eigenschaft
                dbConnection.SecondCommand = "SELECT * FROM Customers";
                Console.WriteLine("SecondCommand value: " + dbConnection.SecondCommand);
                
                // Ändern Sie die SecondCommand, um zu zeigen, dass sie schreibbar ist
                dbConnection.SecondCommand = "SELECT * FROM Orders";
                Console.WriteLine("Updated SecondCommand value: " + dbConnection.SecondCommand);
                
                // Speichere die Arbeitsmappe
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

### Siehe auch

* class [DBConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


