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
// Called: QueryTable queryTable = queryTables[0];
public static void Property_Int32_()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            
            // Access the first worksheet in the workbook
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Access the QueryTableCollection of the worksheet
            QueryTableCollection queryTables = worksheet.QueryTables;
            
            // Display the count of QueryTables in the worksheet
            Console.WriteLine("Number of QueryTables: " + queryTables.Count);
            
            // Set the capacity of the QueryTableCollection
            queryTables.Capacity = 10;
            Console.WriteLine("Capacity of QueryTableCollection: " + queryTables.Capacity);
            
            // Assuming there is at least one QueryTable, access the first QueryTable
            if (queryTables.Count > 0)
            {
                QueryTable queryTable = queryTables[0];
                Console.WriteLine("First QueryTable accessed.");
            }
            else
            {
                Console.WriteLine("No QueryTables found in the worksheet.");
            }
            
            // Save the workbook
            workbook.Save("QueryTableCollectionExample.xlsx");
        }
```

### See Also

* class [QueryTable](../../querytable/)
* class [QueryTableCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


