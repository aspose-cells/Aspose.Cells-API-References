---
title: "Clase WebExtensionBindingCollection"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.WebExtensions.WebExtensionBindingCollection. Representa la lista de relaciones de enlace entre un complemento de Office y los datos del documento"
type: docs
url: /es/net/aspose.cells.webextensions/webextensionbindingcollection/
---
## WebExtensionBindingCollection class

Representa la lista de relaciones de enlace entre un complemento de Office y los datos del documento.

```csharp
public class WebExtensionBindingCollection : CollectionBase<WebExtensionBinding>
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [WebExtensionBindingCollection](webextensionbindingcollection/)() | El constructor predeterminado. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.webextensions/webextensionbindingcollection/item/) { get; } | Obtiene la relación de enlace de extensión web por el índice específico. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [Add](../../aspose.cells.webextensions/webextensionbindingcollection/add/)() | Agrega una relación de enlace entre un complemento de Office y los datos del documento. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(WebExtensionBinding) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(WebExtensionBinding, IComparer&lt;WebExtensionBinding&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, WebExtensionBinding, IComparer&lt;WebExtensionBinding&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(WebExtensionBinding) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(WebExtensionBinding[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(WebExtensionBinding[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, WebExtensionBinding[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;WebExtensionBinding&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;WebExtensionBinding&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;WebExtensionBinding&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;WebExtensionBinding&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;WebExtensionBinding&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;WebExtensionBinding&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;WebExtensionBinding&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;WebExtensionBinding&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;WebExtensionBinding&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;WebExtensionBinding&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(WebExtensionBinding) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(WebExtensionBinding, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(WebExtensionBinding, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(WebExtensionBinding) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(WebExtensionBinding, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(WebExtensionBinding, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.WebExtensions;
    using System;

    public class WebExtensionsClassWebExtensionBindingCollectionDemo
    {
        public static void Run()
        {
            // Cree un nuevo libro de trabajo para la demostración
            Workbook workbook = new Workbook();
            
            try
            {
                // Crear una instancia de WebExtensionBindingCollection
                WebExtensionBindingCollection bindings = new WebExtensionBindingCollection();
                
                // Agregar un nuevo enlace
                int index = bindings.Add();
                
                // Acceder al enlace mediante el indexador
                WebExtensionBinding binding = bindings[index];
                
                // Establecer propiedades en el enlace (asumiendo que estas propiedades existen según los ejemplos de referencia)
                binding.Id = "binding1";
                binding.Type = "table";
                binding.Appref = "Sheet1!A1:B5";
                
                // Mostrar información básica
                Console.WriteLine($"Created binding with ID: {binding.Id}");
                Console.WriteLine($"Total bindings in collection: {bindings.Count}");
                
                // Guarda el libro de trabajo
                workbook.Save("WebExtensionBindingCollectionDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with WebExtensionBindingCollection: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [WebExtensionBinding](../webextensionbinding/)
* namespace [Aspose.Cells.WebExtensions](../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../)


