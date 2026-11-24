---
title: "QueryTable.Name"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "QueryTable‑Eigenschaft. Gibt den Namen der Abfrage‑Tabelle zurück"
type: docs
url: /de/net/aspose.cells/querytable/name/
---
## QueryTable.Name property

Liest den Namen der Abfrage‑Tabelle.

```csharp
public string Name { get; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class QueryTablePropertyNameDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge Beispieldaten hinzu, um eine Abfrage‑Tabelle zu simulieren
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue("John");
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B3"].PutValue("Mary");

            try
            {
                // Prüfe, ob im Arbeitsblatt Abfrage‑Tabellen vorhanden sind.
                if (worksheet.QueryTables.Count > 0)
                {
                    // Hole die erste Abfrage‑Tabelle.
                    QueryTable queryTable = worksheet.QueryTables[0];

                    // Zeige den Wert der Name‑Eigenschaft an (Nur‑Lese‑Operation)
                    Console.WriteLine("Query Table Name: " + queryTable.Name);

                    // Zeige weitere Nur‑Lese‑Eigenschaften zum Kontext an
                    Console.WriteLine("Connection ID: " + queryTable.ConnectionId);
                    Console.WriteLine("Result Range: " + queryTable.ResultRange.Address);
                }
                else
                {
                    Console.WriteLine("No query tables found in the worksheet.");
                }

                // Speichere die Arbeitsmappe
                workbook.Save("QueryTableNameDemo.xlsx");
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


