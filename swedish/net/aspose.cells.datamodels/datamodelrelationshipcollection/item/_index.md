---
title: "DataModelRelationshipCollection.Item"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DataModelRelationshipCollection egenskap. Hämtar relationen"
type: docs
url: /sv/net/aspose.cells.datamodels/datamodelrelationshipcollection/item/
---
## DataModelRelationshipCollection indexer

Hämtar relationen.

```csharp
public DataModelRelationship this[int index] { get; }
```

| Parameter | Beskrivning |
| --- | --- |
| index | Indexet. |

### Exempel

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
            // Skapa en ny arbetsbok (tom datamodell)
            Workbook workbook = new Workbook();

            try
            {
                // Hämta DataModelRelationshipCollection från arbetsboken (kan vara null om ingen datamodell finns)
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
                    // Läs den första relationen med Item (indexerare) egenskapen
                    DataModelRelationship firstRelationship = relationships[0]; // Item property getter
                    Console.WriteLine("First relationship retrieved via Item property:");
                    Console.WriteLine(firstRelationship);
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error while accessing Item property: {ex.Message}");
            }

            // Spara arbetsboken (valfritt, bara för att demonstrera att koden körs från början till slut)
            workbook.Save("ItemPropertyDemo.xlsx");
        }
    }
}
```

### Se även

* class [DataModelRelationship](../../datamodelrelationship/)
* class [DataModelRelationshipCollection](../)
* namespace [Aspose.Cells.DataModels](../../../aspose.cells.datamodels/)
* assembly [Aspose.Cells](../../../)


