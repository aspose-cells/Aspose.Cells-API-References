---
title: QueryTableCollection.Item
second_title: Aspose.Cells for .NET API Reference
description: QueryTableCollection property. Gets the querytable by the specific index
type: docs
url: /net/aspose.cells/querytablecollection/item/
---
## QueryTableCollection indexer

Gets the querytable by the specific index.

```csharp
public QueryTable this[int index] { get; }
```

| Parameter | Description |
| --- | --- |
| index | The index. |

### Return Value

The querytable

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class QueryTableCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();

            // Access the first worksheet
            Worksheet worksheet = workbook.Worksheets[0];

            // Access the QueryTableCollection
            QueryTableCollection queryTables = worksheet.QueryTables;

            try
            {
                // Check if there are any QueryTables
                if (queryTables.Count > 0)
                {
                    // Access the first QueryTable using the Item property
                    QueryTable firstQueryTable = queryTables[0];
                    Console.WriteLine("First QueryTable accessed successfully.");

                    // Display some properties of the QueryTable
                    Console.WriteLine("QueryTable Name: " + firstQueryTable.Name);
                }
                else
                {
                    Console.WriteLine("No QueryTables found in the worksheet.");
                }

                // Save the workbook
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

### See Also

* class [QueryTable](../../querytable/)
* class [QueryTableCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


