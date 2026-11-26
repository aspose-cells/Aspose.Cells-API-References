---
title: "Clase DataModelRelationshipCollection"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.DataModels.DataModelRelationshipCollection clase. Representa las relaciones"
type: docs
url: /es/net/aspose.cells.datamodels/datamodelrelationshipcollection/
---
## DataModelRelationshipCollection class

Representa las relaciones.

```csharp
public class DataModelRelationshipCollection : CollectionBase<DataModelRelationship>
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.datamodels/datamodelrelationshipcollection/item/) { get; } | Obtiene la relación. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Métodos

| Nombre | Descripción |
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

### Ejemplos

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
            // Cree un nuevo libro de trabajo para la demostración
            Workbook workbook = new Workbook();
            
            try
            {
                // Obtener la DataModelRelationshipCollection del modelo de datos del libro
                // Esto asume que el libro tiene un modelo de datos con relaciones
                DataModelRelationshipCollection relationships = workbook.DataModel?.Relationships;
                
                if (relationships == null)
                {
                    Console.WriteLine("Workbook data model doesn't contain relationships");
                    return;
                }
                
                // Demostrar la funcionalidad básica mostrando el recuento
                Console.WriteLine($"Number of relationships: {relationships.Count}");
                
                // Intentar acceder al primer elemento (lanzará una excepción si la colección está vacía)
                try
                {
                    var firstRelationship = relationships[0];
                    Console.WriteLine($"First relationship: {firstRelationship}");
                }
                catch (ArgumentOutOfRangeException)
                {
                    Console.WriteLine("Collection is empty - cannot access items");
                }
                
                // Guarda el libro de trabajo
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

### Ver también

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [DataModelRelationship](../datamodelrelationship/)
* namespace [Aspose.Cells.DataModels](../../aspose.cells.datamodels/)
* assembly [Aspose.Cells](../../)


