---
title: "ExternalConnection.Type"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ExternalConnection property. Liest oder setzt den Typ der externen Verbindungs‑Datenquelle"
type: docs
url: /de/net/aspose.cells.externalconnections/externalconnection/type/
---
## ExternalConnection.Type property

Ruft den externen Verbindungs‑DataSource‑Typ ab oder legt ihn fest.

```csharp
[Obsolete("Use ExternalConnection.SourceType property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public ConnectionDataSourceType Type { get; set; }
```

### Hinweise

HINWEIS: Diese Eigenschaft ist jetzt veraltet. Verwenden Sie stattdessen die Eigenschaft ExternalConnection.SourceType. Diese Eigenschaft wird 12 Monate später, seit Oktober 2024, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionPropertyTypeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            try
            {
                // Greifen Sie auf die erste externe Verbindung zu (sofern eine vorhanden ist)
                ExternalConnection connection = workbook.DataConnections[0];
                
                // Den aktuellen Type-Wert anzeigen (Lesevorgang)
                Console.WriteLine("Initial Type value: " + connection.Type);
                
                // Einen neuen Type-Wert festlegen (da er les- und schreibbar ist)
                connection.Type = ConnectionDataSourceType.OLEDBBasedSource;
                Console.WriteLine("Updated Type value: " + connection.Type);
                
                // Durch mögliche Werte iterieren, um die Einstellungsmöglichkeit zu demonstrieren
                foreach (ConnectionDataSourceType type in Enum.GetValues(typeof(ConnectionDataSourceType)))
                {
                    if ((int)type != 102) // Skip duplicate enum value
                    {
                        connection.Type = type;
                        Console.WriteLine($"Type set to: {type}");
                    }
                }
                
                // Speichern Sie die Arbeitsmappe mit den geänderten Verbindungseinstellungen
                workbook.Save("TypeDemo.xlsx");
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

* enum [ConnectionDataSourceType](../../connectiondatasourcetype/)
* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


