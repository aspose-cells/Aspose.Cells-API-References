---
title: "DataModelRelationshipCollection.Item"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "DataModelRelationshipCollection‑Eigenschaft. Gibt die Beziehung zurück"
type: docs
url: /de/net/aspose.cells.datamodels/datamodelrelationshipcollection/item/
---
## DataModelRelationshipCollection indexer

Liefert die Beziehung.

```csharp
public DataModelRelationship this[int index] { get; }
```

| Parameter | Beschreibung |
| --- | --- |
| Index | Der Index. |

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch (leeres Datenmodell)
            Workbook workbook = new Workbook();

            try
            {
                // Hole die DataModelRelationshipCollection aus dem Arbeitsbuch (kann null sein, wenn kein Datenmodell vorhanden ist)
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
                    // Lese die erste Beziehung über die Item‑Eigenschaft (Indexer)
                    DataModelRelationship firstRelationship = relationships[0]; // Item property getter
                    Console.WriteLine("First relationship retrieved via Item property:");
                    Console.WriteLine(firstRelationship);
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error while accessing Item property: {ex.Message}");
            }

            // Speichere das Arbeitsbuch (optional, nur um zu zeigen, dass der Code End‑zu‑End ausgeführt wird)
            workbook.Save("ItemPropertyDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [DataModelRelationship](../../datamodelrelationship/)
* class [DataModelRelationshipCollection](../)
* namespace [Aspose.Cells.DataModels](../../../aspose.cells.datamodels/)
* assembly [Aspose.Cells](../../../)


