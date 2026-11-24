---
title: "ExternalConnection.BackgroundRefresh"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ExternalConnection‑Eigenschaft. Gibt an, ob die Verbindung im Hintergrund asynchron aktualisiert werden kann. true, wenn die bevorzugte Nutzung der Verbindung darin besteht, asynchron im Hintergrund zu aktualisieren; false, wenn die bevorzugte Nutzung darin besteht, synchron im Vordergrund zu aktualisieren."
type: docs
url: /de/net/aspose.cells.externalconnections/externalconnection/backgroundrefresh/
---
## ExternalConnection.BackgroundRefresh property

Gibt an, ob die Verbindung im Hintergrund (asynchron) aktualisiert werden kann. true, wenn die bevorzugte Nutzung der Verbindung darin besteht, im Hintergrund asynchron zu aktualisieren; false, wenn die bevorzugte Nutzung darin besteht, synchron im Vordergrund zu aktualisieren.

```csharp
public bool BackgroundRefresh { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionPropertyBackgroundRefreshDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            try
            {
                // Greifen Sie auf die erste externe Verbindung zu (sofern eine vorhanden ist)
                ExternalConnection connection = workbook.DataConnections[0];
                
                // Anzeigen des aktuellen BackgroundRefresh-Werts
                Console.WriteLine("Initial BackgroundRefresh value: " + connection.BackgroundRefresh);
                
                // Umschalten des BackgroundRefresh-Werts
                connection.BackgroundRefresh = !connection.BackgroundRefresh;
                Console.WriteLine("Updated BackgroundRefresh value: " + connection.BackgroundRefresh);
                
                // Speichern Sie die Arbeitsmappe mit den geänderten Verbindungseinstellungen
                workbook.Save("BackgroundRefreshDemo.xlsx");
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


