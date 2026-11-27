---
title: "QueryTableCollection.Item"
second_title: "Aspose.Cells för .NET API‑referens"
description: "QueryTableCollection-egenskap. Hämtar frågetabellen med det specifika indexet"
type: docs
url: /sv/net/aspose.cells/querytablecollection/item/
---
## QueryTableCollection indexer

Hämtar querytable efter det specifika indexet.

```csharp
public QueryTable this[int index] { get; }
```

| Parameter | Beskrivning |
| --- | --- |
| index | Indexet. |

### Returvärde

Frågetabellen

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class QueryTableCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];

            // Få åtkomst till QueryTableCollection
            QueryTableCollection queryTables = worksheet.QueryTables;

            try
            {
                // Kontrollera om det finns några QueryTables
                if (queryTables.Count > 0)
                {
                    // Få åtkomst till den första QueryTable med hjälp av Item-egenskapen
                    QueryTable firstQueryTable = queryTables[0];
                    Console.WriteLine("First QueryTable accessed successfully.");

                    // Visa några egenskaper för QueryTable
                    Console.WriteLine("QueryTable Name: " + firstQueryTable.Name);
                }
                else
                {
                    Console.WriteLine("No QueryTables found in the worksheet.");
                }

                // Spara arbetsboken
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

### Se även

* class [QueryTable](../../querytable/)
* class [QueryTableCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


