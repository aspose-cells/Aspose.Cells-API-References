---
title: "DataModel.Relationships"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DataModel egenskap. Hämtar alla relationer för tabellerna i datamodellen"
type: docs
url: /sv/net/aspose.cells.datamodels/datamodel/relationships/
---
## DataModel.Relationships property

Hämtar alla relationer för tabellerna i datamodellen.

```csharp
public DataModelRelationshipCollection Relationships { get; }
```

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            try
            {
                // Få åtkomst till DataModel från arbetsboken
                DataModel dataModel = workbook.DataModel;

                // Visa det aktuella värdet av Relationships-egenskapen (skrivskyddad)
                Console.WriteLine("Number of relationships in DataModel: " + dataModel.Relationships.Count);

                // Iterera genom relationer om några finns
                foreach (DataModelRelationship relationship in dataModel.Relationships)
                {
                    Console.WriteLine("Relationship found: " + relationship);
                }

                // Spara arbetsboken
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

### Se även

* class [DataModelRelationshipCollection](../../datamodelrelationshipcollection/)
* class [DataModel](../)
* namespace [Aspose.Cells.DataModels](../../../aspose.cells.datamodels/)
* assembly [Aspose.Cells](../../../)


