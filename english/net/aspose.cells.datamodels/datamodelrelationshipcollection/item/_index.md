---
title: DataModelRelationshipCollection.Item
second_title: Aspose.Cells for .NET API Reference
description: DataModelRelationshipCollection property. Gets the relationship
type: docs
url: /net/aspose.cells.datamodels/datamodelrelationshipcollection/item/
---
## DataModelRelationshipCollection indexer

Gets the relationship.

```csharp
public DataModelRelationship this[int index] { get; }
```

| Parameter | Description |
| --- | --- |
| index | The index. |

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.DataModels;
    using System;

    public class DataModelRelationshipCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Create a new workbook (empty data model)
            Workbook workbook = new Workbook();

            try
            {
                // Get the DataModelRelationshipCollection from the workbook (may be null if no data model)
                DataModelRelationshipCollection relationships = workbook.DataModel?.Relationships;

                if (relationships == null)
                {
                    Console.WriteLine("The workbook does not contain a data model.");
                }
                else if (relationships.Count == 0)
                {
                    Console.WriteLine("The data model exists but contains no relationships.");
                }
                else
                {
                    // Read the first relationship using the Item (indexer) property
                    DataModelRelationship firstRelationship = relationships[0]; // Item property getter
                    Console.WriteLine("First relationship retrieved via Item property:");
                    Console.WriteLine(firstRelationship);
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error while accessing Item property: {ex.Message}");
            }

            // Save the workbook (optional, just to demonstrate that the code runs end‑to‑end)
            workbook.Save("ItemPropertyDemo.xlsx");
        }
    }
}
```

### See Also

* class [DataModelRelationship](../../datamodelrelationship/)
* class [DataModelRelationshipCollection](../)
* namespace [Aspose.Cells.DataModels](../../../aspose.cells.datamodels/)
* assembly [Aspose.Cells](../../../)


