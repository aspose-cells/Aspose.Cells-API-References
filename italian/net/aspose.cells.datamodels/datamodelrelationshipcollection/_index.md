---
title: "Classe DataModelRelationshipCollection"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.DataModels.DataModelRelationshipCollection. Rappresenta le relazioni"
type: docs
url: /it/net/aspose.cells.datamodels/datamodelrelationshipcollection/
---
## DataModelRelationshipCollection class

Rappresenta le relazioni.

```csharp
public class DataModelRelationshipCollection : CollectionBase<DataModelRelationship>
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.datamodels/datamodelrelationshipcollection/item/) { get; } | Ottiene la relazione. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Metodi

| Nome | Descrizione |
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

### Esempi

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
            // Crea un nuovo workbook per la dimostrazione
            Workbook workbook = new Workbook();
            
            try
            {
                // Ottieni la DataModelRelationshipCollection dal modello dati della cartella di lavoro
                // Questo presuppone che la cartella di lavoro abbia un modello dati con relazioni
                DataModelRelationshipCollection relationships = workbook.DataModel?.Relationships;
                
                if (relationships == null)
                {
                    Console.WriteLine("Workbook data model doesn't contain relationships");
                    return;
                }
                
                // Dimostra la funzionalità di base mostrando il conteggio
                Console.WriteLine($"Number of relationships: {relationships.Count}");
                
                // Prova ad accedere al primo elemento (genererà un'eccezione se la collezione è vuota)
                try
                {
                    var firstRelationship = relationships[0];
                    Console.WriteLine($"First relationship: {firstRelationship}");
                }
                catch (ArgumentOutOfRangeException)
                {
                    Console.WriteLine("Collection is empty - cannot access items");
                }
                
                // Salva la cartella di lavoro
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

### Vedi anche

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [DataModelRelationship](../datamodelrelationship/)
* namespace [Aspose.Cells.DataModels](../../aspose.cells.datamodels/)
* assembly [Aspose.Cells](../../)


