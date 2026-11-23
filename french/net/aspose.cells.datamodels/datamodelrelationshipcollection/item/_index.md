---
title: "DataModelRelationshipCollection.Item"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété DataModelRelationshipCollection. Obtient la relation"
type: docs
url: /fr/net/aspose.cells.datamodels/datamodelrelationshipcollection/item/
---
## DataModelRelationshipCollection indexer

Obtient la relation.

```csharp
public DataModelRelationship this[int index] { get; }
```

| Paramètre | Description |
| --- | --- |
| indice | L'indice. |

### Exemples

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
            // Créer un nouveau classeur (modèle de données vide)
            Workbook workbook = new Workbook();

            try
            {
                // Obtenez la DataModelRelationshipCollection du classeur (peut être null si aucun modèle de données)
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
                    // Lire la première relation en utilisant la propriété Item (indexeur)
                    DataModelRelationship firstRelationship = relationships[0]; // Item property getter
                    Console.WriteLine("First relationship retrieved via Item property:");
                    Console.WriteLine(firstRelationship);
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error while accessing Item property: {ex.Message}");
            }

            // Enregistrer le classeur (optionnel, juste pour démontrer que le code s'exécute de bout en bout)
            workbook.Save("ItemPropertyDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [DataModelRelationship](../../datamodelrelationship/)
* class [DataModelRelationshipCollection](../)
* namespace [Aspose.Cells.DataModels](../../../aspose.cells.datamodels/)
* assembly [Aspose.Cells](../../../)


