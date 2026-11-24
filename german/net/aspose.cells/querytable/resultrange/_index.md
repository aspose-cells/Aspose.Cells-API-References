---
title: "QueryTable.ResultRange"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "QueryTable‑Eigenschaft. Gibt den Ergebnisbereich zurück"
type: docs
url: /de/net/aspose.cells/querytable/resultrange/
---
## QueryTable.ResultRange property

Liest den Bereich des Ergebnisses.

```csharp
public Range ResultRange { get; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class QueryTablePropertyResultRangeDemo
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

                    // Zeige den Wert der ResultRange‑Eigenschaft an (Nur‑Lese‑Operation)
                    Aspose.Cells.Range resultRange = queryTable.ResultRange;
                    Console.WriteLine("ResultRange Address: " + resultRange.Address);
                    Console.WriteLine("ResultRange Row Count: " + resultRange.RowCount);
                    Console.WriteLine("ResultRange Column Count: " + resultRange.ColumnCount);
                    Console.WriteLine("ResultRange First Row: " + resultRange.FirstRow);
                    Console.WriteLine("ResultRange First Column: " + resultRange.FirstColumn);

                    // Zeige die Werte im Ergebnisbereich an
                    Console.WriteLine("Values in ResultRange:");
                    foreach (Cell cell in resultRange)
                    {
                        Console.WriteLine($"Cell [{cell.Row}, {cell.Column}]: {cell.Value}");
                    }
                }
                else
                {
                    Console.WriteLine("No query tables found in the worksheet.");
                }

                // Speichere die Arbeitsmappe
                workbook.Save("ResultRangeDemo.xlsx");
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

* class [Range](../../range/)
* class [QueryTable](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


