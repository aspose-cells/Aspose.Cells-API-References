---
title: "QueryTableCollection.Item"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "QueryTableCollection‑Eigenschaft. Gibt die Abfrage‑Tabelle anhand des angegebenen Index zurück."
type: docs
url: /de/net/aspose.cells/querytablecollection/item/
---
## QueryTableCollection indexer

Liest die QueryTable anhand des angegebenen Index.

```csharp
public QueryTable this[int index] { get; }
```

| Parameter | Beschreibung |
| --- | --- |
| Index | Der Index. |

### Rückgabewert

Die QueryTable

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class QueryTableCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];

            // Greifen Sie auf die QueryTableCollection zu
            QueryTableCollection queryTables = worksheet.QueryTables;

            try
            {
                // Prüfen Sie, ob QueryTables vorhanden sind
                if (queryTables.Count > 0)
                {
                    // Greifen Sie über die Item-Eigenschaft auf die erste QueryTable zu
                    QueryTable firstQueryTable = queryTables[0];
                    Console.WriteLine("First QueryTable accessed successfully.");

                    // Zeigen Sie einige Eigenschaften der QueryTable an
                    Console.WriteLine("QueryTable Name: " + firstQueryTable.Name);
                }
                else
                {
                    Console.WriteLine("No QueryTables found in the worksheet.");
                }

                // Speichere die Arbeitsmappe
                workbook.Save("QueryTableItemDemo.xlsx");
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

* class [QueryTable](../../querytable/)
* class [QueryTableCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


