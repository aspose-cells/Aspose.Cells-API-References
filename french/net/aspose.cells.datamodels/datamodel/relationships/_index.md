---
title: "DataModel.Relationships"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété DataModel. Obtient toutes les relations des tables dans le modèle de données"
type: docs
url: /fr/net/aspose.cells.datamodels/datamodel/relationships/
---
## DataModel.Relationships property

Obtient toutes les relations des tables du modèle de données.

```csharp
public DataModelRelationshipCollection Relationships { get; }
```

### Exemples

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
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            try
            {
                // Accéder au DataModel depuis le classeur
                DataModel dataModel = workbook.DataModel;

                // Afficher la valeur actuelle de la propriété Relationships (lecture seule)
                Console.WriteLine("Number of relationships in DataModel: " + dataModel.Relationships.Count);

                // Itérer à travers les relations si elles existent
                foreach (DataModelRelationship relationship in dataModel.Relationships)
                {
                    Console.WriteLine("Relationship found: " + relationship);
                }

                // Enregistrez le classeur
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

### Voir aussi

* class [DataModelRelationshipCollection](../../datamodelrelationshipcollection/)
* class [DataModel](../)
* namespace [Aspose.Cells.DataModels](../../../aspose.cells.datamodels/)
* assembly [Aspose.Cells](../../../)


