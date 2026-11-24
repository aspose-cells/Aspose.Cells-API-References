---
title: "ExternalConnection.SecondCommand"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ExternalConnection-Eigenschaft. Gibt eine zweite Befehlszeichenfolge an, die erhalten bleibt, wenn serverbasierte Seitenfelder der PivotTable verwendet werden. Für ODBC-Verbindungen ist serverCommand in der Regel eine umfassendere Abfrage als command, da im ersteren keine WHERE-Klausel vorhanden ist. Auf Basis dieser beiden Befehle, Command und ServerCommand, kann die Parameter‑UI gefüllt und parametrische Abfragen erstellt werden."
type: docs
url: /de/net/aspose.cells.externalconnections/externalconnection/secondcommand/
---
## ExternalConnection.SecondCommand property

Gibt eine zweite Befehlszeichenfolge an, die gespeichert wird, wenn serverbasierte Seitenfelder einer PivotTable verwendet werden. Für ODBC-Verbindungen ist serverCommand in der Regel eine umfangreichere Abfrage als command (es ist keine WHERE‑Klausel in ersterer enthalten). Basierend auf diesen beiden Befehlen (Command und ServerCommand) kann die Parameter‑UI gefüllt und parametrisierte Abfragen erstellt werden

```csharp
public virtual string SecondCommand { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionPropertySecondCommandDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            try
            {
                // Greifen Sie auf die erste externe Verbindung zu (sofern eine vorhanden ist)
                ExternalConnection connection = workbook.DataConnections[0];
                
                // Zeige den aktuellen SecondCommand-Wert an (Lesevorgang).
                Console.WriteLine("Initial SecondCommand value: " + connection.SecondCommand);
                
                // Setze einen neuen SecondCommand-Wert (da er les- und schreibbar ist).
                connection.SecondCommand = "SELECT * FROM Customers WHERE Country = 'USA'";
                Console.WriteLine("Updated SecondCommand value: " + connection.SecondCommand);
                
                // Leere den SecondCommand, um das Setzen einer leeren Zeichenkette zu demonstrieren.
                connection.SecondCommand = string.Empty;
                Console.WriteLine("Cleared SecondCommand value: " + connection.SecondCommand);
                
                // Speichern Sie die Arbeitsmappe mit den geänderten Verbindungseinstellungen
                workbook.Save("SecondCommandDemo.xlsx");
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

* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


