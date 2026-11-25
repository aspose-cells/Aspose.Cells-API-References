---
title: "QueryTableCollection.Item"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà QueryTableCollection. Ottiene la querytable tramite l'indice specifico"
type: docs
url: /it/net/aspose.cells/querytablecollection/item/
---
## QueryTableCollection indexer

Restituisce la querytable mediante l'indice specifico.

```csharp
public QueryTable this[int index] { get; }
```

| Parametro | Descrizione |
| --- | --- |
| indice | L'indice. |

### Valore di ritorno

La querytable

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class QueryTableCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Accedi a QueryTableCollection
            QueryTableCollection queryTables = worksheet.QueryTables;

            try
            {
                // Verifica se ci sono QueryTables
                if (queryTables.Count > 0)
                {
                    // Accedi al primo QueryTable usando la proprietà Item
                    QueryTable firstQueryTable = queryTables[0];
                    Console.WriteLine("First QueryTable accessed successfully.");

                    // Mostra alcune proprietà del QueryTable
                    Console.WriteLine("QueryTable Name: " + firstQueryTable.Name);
                }
                else
                {
                    Console.WriteLine("No QueryTables found in the worksheet.");
                }

                // Salva la cartella di lavoro
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

### Vedi anche

* class [QueryTable](../../querytable/)
* class [QueryTableCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


