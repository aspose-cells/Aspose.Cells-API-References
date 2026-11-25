---
title: "DataModel.Relationships"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà DataModel. Ottiene tutte le relazioni delle tabelle nel modello dati"
type: docs
url: /it/net/aspose.cells.datamodels/datamodel/relationships/
---
## DataModel.Relationships property

Ottiene tutte le relazioni delle tabelle nel modello dati.

```csharp
public DataModelRelationshipCollection Relationships { get; }
```

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            try
            {
                // Accedi al DataModel dalla cartella di lavoro
                DataModel dataModel = workbook.DataModel;

                // Visualizza il valore corrente della proprietà Relationships (sola lettura)
                Console.WriteLine("Number of relationships in DataModel: " + dataModel.Relationships.Count);

                // Itera attraverso le relazioni se ne esistono
                foreach (DataModelRelationship relationship in dataModel.Relationships)
                {
                    Console.WriteLine("Relationship found: " + relationship);
                }

                // Salva la cartella di lavoro
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

### Vedi anche

* class [DataModelRelationshipCollection](../../datamodelrelationshipcollection/)
* class [DataModel](../)
* namespace [Aspose.Cells.DataModels](../../../aspose.cells.datamodels/)
* assembly [Aspose.Cells](../../../)


