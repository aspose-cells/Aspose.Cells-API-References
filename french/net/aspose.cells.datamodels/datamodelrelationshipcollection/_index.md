---
title: "Classe DataModelRelationshipCollection"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.DataModels.DataModelRelationshipCollection classe. Représente les relations"
type: docs
url: /fr/net/aspose.cells.datamodels/datamodelrelationshipcollection/
---
## DataModelRelationshipCollection class

Représente les relations.

```csharp
public class DataModelRelationshipCollection : CollectionBase<DataModelRelationship>
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.datamodels/datamodelrelationshipcollection/item/) { get; } | Obtient la relation. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Méthodes

| Nom | Description |
| --- | --- |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(DataModelRelationship) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(DataModelRelationship, IComparer&lt;DataModelRelationship&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, DataModelRelationship, IComparer&lt;DataModelRelationship&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(DataModelRelationship) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(DataModelRelationship[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(DataModelRelationship[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, DataModelRelationship[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;DataModelRelationship&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;DataModelRelationship&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;DataModelRelationship&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;DataModelRelationship&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;DataModelRelationship&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;DataModelRelationship&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;DataModelRelationship&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;DataModelRelationship&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;DataModelRelationship&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;DataModelRelationship&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(DataModelRelationship) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(DataModelRelationship, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(DataModelRelationship, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(DataModelRelationship) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(DataModelRelationship, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(DataModelRelationship, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.DataModels;
    using System;

    public class DataModelsClassDataModelRelationshipCollectionDemo
    {
        public static void Run()
        {
            // Créez un nouveau classeur pour la démonstration
            Workbook workbook = new Workbook();
            
            try
            {
                // Obtenir la DataModelRelationshipCollection du modèle de données du classeur
                // Cela suppose que le classeur possède un modèle de données avec des relations
                DataModelRelationshipCollection relationships = workbook.DataModel?.Relationships;
                
                if (relationships == null)
                {
                    Console.WriteLine("Workbook data model doesn't contain relationships");
                    return;
                }
                
                // Démontrer la fonctionnalité de base en affichant le nombre
                Console.WriteLine($"Number of relationships: {relationships.Count}");
                
                // Essayer d'accéder au premier élément (générera une exception si la collection est vide)
                try
                {
                    var firstRelationship = relationships[0];
                    Console.WriteLine($"First relationship: {firstRelationship}");
                }
                catch (ArgumentOutOfRangeException)
                {
                    Console.WriteLine("Collection is empty - cannot access items");
                }
                
                // Enregistrez le classeur
                workbook.Save("DataModelRelationshipCollectionDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with DataModelRelationshipCollection: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [DataModelRelationship](../datamodelrelationship/)
* namespace [Aspose.Cells.DataModels](../../aspose.cells.datamodels/)
* assembly [Aspose.Cells](../../)


