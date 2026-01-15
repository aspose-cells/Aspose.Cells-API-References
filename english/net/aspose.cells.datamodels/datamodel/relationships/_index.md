---
title: DataModel.Relationships
second_title: Aspose.Cells for .NET API Reference
description: DataModel property. Gets all relationships of the tables in the data model
type: docs
url: /net/aspose.cells.datamodels/datamodel/relationships/
---
## DataModel.Relationships property

Gets all relationships of the tables in the data model.

```csharp
public DataModelRelationshipCollection Relationships { get; }
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.DataModels;
    using System;

    public class DataModelPropertyRelationshipsDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();

            try
            {
                // Access the DataModel from the workbook
                DataModel dataModel = workbook.DataModel;

                // Display the current value of the Relationships property (read-only)
                Console.WriteLine("Number of relationships in DataModel: " + dataModel.Relationships.Count);

                // Iterate through relationships if any exist
                foreach (DataModelRelationship relationship in dataModel.Relationships)
                {
                    Console.WriteLine("Relationship found: " + relationship);
                }

                // Save the workbook
                workbook.Save("RelationshipsDemo.xlsx");
                Console.WriteLine("Relationships demonstration completed successfully.");
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

* class [DataModelRelationshipCollection](../../datamodelrelationshipcollection/)
* class [DataModel](../)
* namespace [Aspose.Cells.DataModels](../../../aspose.cells.datamodels/)
* assembly [Aspose.Cells](../../../)


