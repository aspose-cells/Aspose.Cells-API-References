---
title: "ExternalConnection.ConnectionId"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ExternalConnection property. Gibt die eindeutige Kennung dieser Verbindung an"
type: docs
url: /de/net/aspose.cells.externalconnections/externalconnection/connectionid/
---
## ExternalConnection.ConnectionId property

Gibt die eindeutige Kennung dieser Verbindung an.

```csharp
[Obsolete("Use ExternalConnection.Id property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int ConnectionId { get; }
```

### Hinweise

HINWEIS: Diese Eigenschaft ist jetzt veraltet. Stattdessen verwenden Sie bitte die Eigenschaft ExternalConnection.Id. Diese Eigenschaft wird 12 Monate später, seit Oktober 2024, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erlebt haben.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionPropertyConnectionIdDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            try
            {
                // Greifen Sie auf die erste externe Verbindung zu (die Arbeitsmappe enthält Standardverbindungen)
                ExternalConnection connection = workbook.DataConnections[0];

                // Zeigen Sie den ConnectionId-Wert an (schreibgeschützte Eigenschaft)
                Console.WriteLine("ConnectionId value: " + connection.ConnectionId);

                // Zeigen Sie den Id-Wert zum Vergleich an (ebenfalls schreibgeschützt)
                Console.WriteLine("Id value: " + connection.Id);

                // Zeigen Sie, dass beide Eigenschaften schreibgeschützt sind, indem Sie versuchen, sie anzuzeigen
                Console.WriteLine("ConnectionId and Id are both read-only properties");
                Console.WriteLine("ConnectionId: " + connection.ConnectionId + ", Id: " + connection.Id);

                // Speichere die Arbeitsmappe
                workbook.Save("ConnectionIdDemo.xlsx");
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


