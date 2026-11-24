---
title: "Workbook.DataConnections"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Workbook property. Gets the ExternalConnection collection"
type: docs
url: /de/net/aspose.cells/workbook/dataconnections/
---
## Workbook.DataConnections property

Ruft die [`ExternalConnection`](../../../aspose.cells.externalconnections/externalconnection/) Sammlung ab.

```csharp
public ExternalConnectionCollection DataConnections { get; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorkbookPropertyDataConnectionsDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Erstelle ein Beispiel-Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge einige Daten hinzu, um das Beispiel sinnvoll zu machen.
            worksheet.Cells["A1"].Value = "Sample Data";

            try
            {
                // Greifen Sie auf die DataConnections-Eigenschaft zu
                var dataConnections = workbook.DataConnections;

                // Zeigen Sie den aktuellen Wert der Eigenschaft an (Lesevorgang)
                Console.WriteLine("DataConnections count: " + dataConnections.Count);

                // Iterieren Sie über die Verbindungen, falls welche vorhanden sind
                for (int i = 0; i < dataConnections.Count; i++)
                {
                    var connection = dataConnections[i];
                    Console.WriteLine($"Connection {i + 1}: {connection.Name}");
                }

                // Zeigen, wie die Eigenschaft das Verhalten beeinflusst
                Console.WriteLine("DataConnections has been demonstrated");

                // Ergebnis speichern
                workbook.Save("DataConnectionsDemo.xlsx");
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

* class [ExternalConnectionCollection](../../../aspose.cells.externalconnections/externalconnectioncollection/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


