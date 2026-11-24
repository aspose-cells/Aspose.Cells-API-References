---
title: "WorksheetCollection.IsRefreshAllConnections"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WorksheetCollection-Eigenschaft. Gibt an, ob beim Öffnen der Datei in MS Excel alle Verbindungen aktualisiert werden"
type: docs
url: /de/net/aspose.cells/worksheetcollection/isrefreshallconnections/
---
## WorksheetCollection.IsRefreshAllConnections property

Gibt an, ob beim Öffnen der Datei in MS Excel alle Verbindungen aktualisiert werden.

```csharp
public bool IsRefreshAllConnections { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionPropertyIsRefreshAllConnectionsDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greift auf die Arbeitsblatt‑Sammlung zu
            WorksheetCollection worksheets = workbook.Worksheets;
            
            // Füge einige Beispielarbeitsblätter hinzu
            worksheets.Add("Sheet1");
            worksheets.Add("Sheet2");
            
            // Setze die IsRefreshAllConnections-Eigenschaft
            worksheets.IsRefreshAllConnections = true;
            
            // Zeige den aktuellen Wert von IsRefreshAllConnections an
            Console.WriteLine("IsRefreshAllConnections: " + worksheets.IsRefreshAllConnections);
            
            // Speichere die Arbeitsmappe
            workbook.Save("WorksheetCollectionPropertyIsRefreshAllConnectionsDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


