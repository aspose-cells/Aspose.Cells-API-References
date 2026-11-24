---
title: "QueryTable.ExternalConnection"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "QueryTable‑Eigenschaft. Gibt die zugehörige externe Verbindung zurück"
type: docs
url: /de/net/aspose.cells/querytable/externalconnection/
---
## QueryTable.ExternalConnection property

Liest die zugehörige externe Verbindung.

```csharp
public ExternalConnection ExternalConnection { get; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class QueryTablePropertyExternalConnectionDemo
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

                    // Greife auf die ExternalConnection‑Eigenschaft zu (Nur‑Lese)
                    ExternalConnection externalConnection = queryTable.ExternalConnection;

                    // Zeige Informationen zur externen Verbindung an
                    if (externalConnection != null)
                    {
                        Console.WriteLine("External Connection ID: " + externalConnection.Id);
                        Console.WriteLine("External Connection Name: " + externalConnection.Name);
                        Console.WriteLine("External Connection Type: " + externalConnection.ClassType);
                        Console.WriteLine("Connection String: " + externalConnection.ConnectionString);
                        Console.WriteLine("Refresh on Load: " + externalConnection.RefreshOnLoad);
                    }
                    else
                    {
                        Console.WriteLine("No external connection associated with this query table.");
                    }

                    // Zeige weitere Abfrage‑Tabellen‑Eigenschaften zum Kontext an
                    Console.WriteLine("Query Table Name: " + queryTable.Name);
                    Console.WriteLine("Connection ID: " + queryTable.ConnectionId);
                }
                else
                {
                    Console.WriteLine("No query tables found in the worksheet.");
                }

                // Speichere die Arbeitsmappe
                workbook.Save("ExternalConnectionDemo.xlsx");
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

* class [ExternalConnection](../../../aspose.cells.externalconnections/externalconnection/)
* class [QueryTable](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


