---
title: "Workbook.DataMashup"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Workbook-Eigenschaft. Ruft Mashup-Daten ab"
type: docs
url: /de/net/aspose.cells/workbook/datamashup/
---
## Workbook.DataMashup property

Liest Mashup-Daten.

```csharp
public DataMashup DataMashup { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.ExternalConnections;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyDataMashupDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe mit Beispieldaten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Beispieldaten hinzufügen, um Power Query auszulösen
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B3"].PutValue(150);

            // In einer Datei speichern
            string sourcePath = "source.xlsx";
            workbook.Save(sourcePath);

            // Arbeitsmappe erneut öffnen, um auf DataMashup zuzugreifen
            workbook = new Workbook(sourcePath);
            
            // Zugriff auf Power Query-Formeln über die DataMashup-Eigenschaft
            var queries = workbook.DataMashup.PowerQueryFormulas;
            
            // Grundlegende Informationen zu Abfragen ausgeben
            Console.WriteLine($"Number of Power Query formulas: {queries.Count}");
            
            // Falls Abfragen vorhanden sind, Details der ersten anzeigen
            if (queries.Count > 0)
            {
                foreach (var query in queries)
                {
                    Console.WriteLine($"Query Name: {query.Name}");
                    Console.WriteLine($"Number of items: {query.PowerQueryFormulaItems.Count}");
                    break; // Just show first query for demo
                }
            }

            // In einer neuen Datei speichern
            string destPath = "output.xlsx";
            workbook.Save(destPath);
        }
    }
}
```

### Siehe auch

* class [DataMashup](../../../aspose.cells.querytables/datamashup/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


