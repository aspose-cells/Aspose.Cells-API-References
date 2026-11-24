---
title: "QueryTable.ConnectionId"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "QueryTable‑Eigenschaft. Gibt die connection id der Abfrage‑Tabelle zurück"
type: docs
url: /de/net/aspose.cells/querytable/connectionid/
---
## QueryTable.ConnectionId property

Liest die Verbindungs-ID der Abfrage‑Tabelle.

```csharp
public int ConnectionId { get; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class QueryTablePropertyConnectionIdDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge Beispieldaten hinzu, um ein Abfrage‑Tabellen‑Szenario zu simulieren
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue("Sample Data");

            try
            {
                // Prüfe, ob im Arbeitsblatt Abfrage‑Tabellen vorhanden sind.
                if (worksheet.QueryTables.Count > 0)
                {
                    // Hole die erste Abfrage‑Tabelle.
                    QueryTable queryTable = worksheet.QueryTables[0];

                    // Zeige den Wert der ConnectionId‑Eigenschaft an (Nur‑Lese)
                    Console.WriteLine("Query Table ConnectionId: " + queryTable.ConnectionId);

                    // Andere verwandte Eigenschaften im Kontext anzeigen
                    Console.WriteLine("Query Table Name: " + queryTable.Name);
                    Console.WriteLine("External Connection: " +
                        (queryTable.ExternalConnection != null ? queryTable.ExternalConnection.Name : "None"));
                }
                else
                {
                    Console.WriteLine("No query tables found in the worksheet.");
                }

                // Speichere die Arbeitsmappe
                workbook.Save("ConnectionIdDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
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

* class [QueryTable](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


