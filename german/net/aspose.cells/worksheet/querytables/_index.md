---
title: "Worksheet.QueryTables"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Worksheet-Eigenschaft. Ruft die QueryTableCollection im Arbeitsblatt ab"
type: docs
url: /de/net/aspose.cells/worksheet/querytables/
---
## Worksheet.QueryTables property

Ruft [`QueryTableCollection`](../../querytablecollection/) im Arbeitsblatt ab.

```csharp
public QueryTableCollection QueryTables { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyQueryTablesDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(2.5);
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B3"].PutValue(1.8);
            
            // Rufen Sie die erste Abfrage‑Tabelle ab (da wir keine neuen direkt hinzufügen können)
            // Hinweis: Die QueryTables-Sammlung ist in dieser API-Version schreibgeschützt.
            if (worksheet.QueryTables.Count > 0)
            {
                QueryTable queryTable = worksheet.QueryTables[0];
                
                // Abfrage-Tabelleninformationen anzeigen
                Console.WriteLine("Query Table Name: " + queryTable.Name);
                Console.WriteLine("Result Range: " + queryTable.ResultRange.Address);
                Console.WriteLine("Number of Query Tables: " + worksheet.QueryTables.Count);
            }
            else
            {
                Console.WriteLine("No query tables found in the worksheet.");
            }
            
            // Speichere die Arbeitsmappe
            workbook.Save("QueryTableDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [QueryTableCollection](../../querytablecollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


