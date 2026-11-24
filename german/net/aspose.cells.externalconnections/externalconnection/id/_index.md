---
title: "ExternalConnection.Id"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ExternalConnection property. Gibt die ID der Verbindung zurück"
type: docs
url: /de/net/aspose.cells.externalconnections/externalconnection/id/
---
## ExternalConnection.Id property

Ermittelt die ID der Verbindung.

```csharp
public int Id { get; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionPropertyIdDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            try
            {
                // Greifen Sie auf die erste externe Verbindung zu (die Arbeitsmappe enthält Standardverbindungen)
                ExternalConnection connection = workbook.DataConnections[0];

                // Zeigen Sie den aktuellen Id-Wert an (schreibgeschützte Eigenschaft)
                Console.WriteLine("External Connection Id: " + connection.Id);

                // Zeige weitere Nur‑Lese‑Eigenschaften zum Kontext an
                Console.WriteLine("Connection Class Type: " + connection.ClassType);
                Console.WriteLine("Connection Name: " + connection.Name);

                // Speichere die Arbeitsmappe
                workbook.Save("ExternalConnectionIdDemo.xlsx");
                Console.WriteLine("Workbook saved successfully with connection Id: " + connection.Id);
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


