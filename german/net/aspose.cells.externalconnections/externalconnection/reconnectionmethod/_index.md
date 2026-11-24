---
title: "ExternalConnection.ReconnectionMethod"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ExternalConnection‑Eigenschaft. Gibt an, was die Tabellenkalkulationsanwendung tun soll, wenn eine Verbindung fehlschlägt. Der Standardwert ist ReConnectionMethodType.Required"
type: docs
url: /de/net/aspose.cells.externalconnections/externalconnection/reconnectionmethod/
---
## ExternalConnection.ReconnectionMethod property

Gibt an, was die Tabellenkalkulationsanwendung tun soll, wenn eine Verbindung fehlschlägt. Der Standardwert ist ReConnectionMethodType.Required.

```csharp
[Obsolete("Use ExternalConnection.ReconnectionMethodType property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public ReConnectionMethodType ReconnectionMethod { get; set; }
```

### Hinweise

HINWEIS: Diese Eigenschaft ist jetzt veraltet. Verwenden Sie stattdessen die Eigenschaft ExternalConnection.ReconnectionMethodType. Diese Eigenschaft wird 12 Monate später, seit Oktober 2017, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionPropertyReconnectionMethodDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            try
            {
                // Greifen Sie auf die erste externe Verbindung zu (sofern eine vorhanden ist)
                ExternalConnection connection = workbook.DataConnections[0];
                
                // Anzeigen des aktuellen ReconnectionMethod-Werts (Lesevorgang)
                Console.WriteLine("Initial ReconnectionMethod value: " + connection.ReconnectionMethod);
                
                // Setze neue ReconnectionMethod-Werte (da sie les- und schreibbar ist)
                connection.ReconnectionMethod = ReConnectionMethodType.Always;
                Console.WriteLine("Updated ReconnectionMethod value: " + connection.ReconnectionMethod);
                
                connection.ReconnectionMethod = ReConnectionMethodType.Never;
                Console.WriteLine("Updated ReconnectionMethod value: " + connection.ReconnectionMethod);
                
                // Auf den Standardwert zurücksetzen
                connection.ReconnectionMethod = ReConnectionMethodType.Required;
                Console.WriteLine("Reset ReconnectionMethod value: " + connection.ReconnectionMethod);
                
                // Speichern Sie die Arbeitsmappe mit den geänderten Verbindungseinstellungen
                workbook.Save("ReconnectionMethodDemo.xlsx");
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

* enum [ReConnectionMethodType](../../reconnectionmethodtype/)
* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


