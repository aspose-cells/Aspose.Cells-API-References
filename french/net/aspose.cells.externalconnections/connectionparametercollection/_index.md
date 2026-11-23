---
title: "Classe ConnectionParameterCollection"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.ExternalConnections.ConnectionParameterCollection. Spécifie la collection ConnectionParameter"
type: docs
url: /fr/net/aspose.cells.externalconnections/connectionparametercollection/
---
## ConnectionParameterCollection class

Spécifie la collection [`ConnectionParameter`](../connectionparameter/)

```csharp
public class ConnectionParameterCollection : CollectionBase<ConnectionParameter>
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.externalconnections/connectionparametercollection/item/) { get; } | Obtient l'élément [`ConnectionParameter`](../connectionparameter/) à l'index spécifié. (2 indexeurs) |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Méthodes

| Nom | Description |
| --- | --- |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(ConnectionParameter) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(ConnectionParameter, IComparer&lt;ConnectionParameter&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, ConnectionParameter, IComparer&lt;ConnectionParameter&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(ConnectionParameter) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(ConnectionParameter[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(ConnectionParameter[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, ConnectionParameter[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;ConnectionParameter&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;ConnectionParameter&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;ConnectionParameter&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;ConnectionParameter&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;ConnectionParameter&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;ConnectionParameter&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;ConnectionParameter&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;ConnectionParameter&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;ConnectionParameter&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;ConnectionParameter&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(ConnectionParameter) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(ConnectionParameter, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(ConnectionParameter, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(ConnectionParameter) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(ConnectionParameter, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(ConnectionParameter, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionsClassConnectionParameterCollectionDemo
    {
        public static void Run()
        {
            // Créez un nouveau classeur pour la démonstration
            Workbook workbook = new Workbook();
            
            try
            {
                // Obtenir la première connexion externe (en créera une si aucune n'existe)
                ExternalConnection connection = workbook.DataConnections[0];
                
                // Obtenir la collection de paramètres de la connexion
                ConnectionParameterCollection parameters = connection.Parameters;
                
                // Démontrer la fonctionnalité de base en vérifiant les propriétés de la collection
                Console.WriteLine($"ConnectionParameterCollection count: {parameters.Count}");
                
                // Tenter d'accéder à un élément (sera nul si la collection est vide)
                if (parameters.Count > 0)
                {
                    ConnectionParameter param = parameters[0];
                    Console.WriteLine(param == null ? "No parameters in collection" : "Parameter exists");
                }
                else
                {
                    Console.WriteLine("No parameters in collection");
                }
                
                // Enregistrez le classeur
                workbook.Save("ConnectionParameterCollectionDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with ConnectionParameterCollection: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [ConnectionParameter](../connectionparameter/)
* namespace [Aspose.Cells.ExternalConnections](../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../)


