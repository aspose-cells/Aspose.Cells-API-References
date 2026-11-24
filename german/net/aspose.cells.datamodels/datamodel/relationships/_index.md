---
title: "DataModel.Relationships"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "DataModel-Eigenschaft. Ruft alle Beziehungen der Tabellen im Datemodell ab"
type: docs
url: /de/net/aspose.cells.datamodels/datamodel/relationships/
---
## DataModel.Relationships property

Liefert alle Beziehungen der Tabellen im Datenmodell.

```csharp
public DataModelRelationshipCollection Relationships { get; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            try
            {
                // Greifen Sie auf das DataModel aus der Arbeitsmappe zu
                DataModel dataModel = workbook.DataModel;

                // Zeigen Sie den aktuellen Wert der Relationships-Eigenschaft (schreibgeschützt) an
                Console.WriteLine("Number of relationships in DataModel: " + dataModel.Relationships.Count);

                // Durchlaufen Sie die Beziehungen, falls welche existieren
                foreach (DataModelRelationship relationship in dataModel.Relationships)
                {
                    Console.WriteLine("Relationship found: " + relationship);
                }

                // Speichere die Arbeitsmappe
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

### Siehe auch

* class [DataModelRelationshipCollection](../../datamodelrelationshipcollection/)
* class [DataModel](../)
* namespace [Aspose.Cells.DataModels](../../../aspose.cells.datamodels/)
* assembly [Aspose.Cells](../../../)


