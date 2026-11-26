---
title: "Clase CustomDocumentPropertyCollection"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.Properties.CustomDocumentPropertyCollection class. Una colección de propiedades de documento personalizadas"
type: docs
url: /es/net/aspose.cells.properties/customdocumentpropertycollection/
---
## CustomDocumentPropertyCollection class

Una colección de propiedades de documento personalizadas.

```csharp
public class CustomDocumentPropertyCollection : DocumentPropertyCollection
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.properties/documentpropertycollection/item/) { get; } | Devuelve un objeto [`DocumentProperty`](../documentproperty/) por índice.(Herencia de [`DocumentPropertyCollection`](../documentpropertycollection/).) |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |
| virtual [Item](../../aspose.cells.properties/documentpropertycollection/item/) { get; } | Devuelve un objeto [`DocumentProperty`](../documentproperty/) por el nombre de la propiedad.(Heredado de [`DocumentPropertyCollection`](../documentpropertycollection/).) |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [Add](../../aspose.cells.properties/customdocumentpropertycollection/add/#add)(string, bool) | Crea una nueva propiedad de documento personalizada del tipo de datos **PropertyType.Boolean**. |
| [Add](../../aspose.cells.properties/customdocumentpropertycollection/add/#add_3)(string, DateTime) | Crea una nueva propiedad de documento personalizada del tipo de datos **PropertyType.DateTime**. |
| [Add](../../aspose.cells.properties/customdocumentpropertycollection/add/#add_1)(string, double) | Crea una nueva propiedad de documento personalizada del tipo de datos **PropertyType.Float**. |
| [Add](../../aspose.cells.properties/customdocumentpropertycollection/add/#add_2)(string, int) | Crea una nueva propiedad de documento personalizada del tipo de datos **PropertyType.Number**. |
| [Add](../../aspose.cells.properties/customdocumentpropertycollection/add/#add_4)(string, string) | Crea una nueva propiedad de documento personalizada del tipo de datos **PropertyType.String**. |
| [AddLinkToContent](../../aspose.cells.properties/customdocumentpropertycollection/addlinktocontent/)(string, string) | Crea una nueva propiedad de documento personalizada que enlaza con contenido. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(DocumentProperty) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(DocumentProperty, IComparer&lt;DocumentProperty&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, DocumentProperty, IComparer&lt;DocumentProperty&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(DocumentProperty) |  |
| [Contains](../../aspose.cells.properties/documentpropertycollection/contains/)(string) | Devuelve true si una propiedad con el nombre especificado existe en la colección.(Heredado de [`DocumentPropertyCollection`](../documentpropertycollection/).) |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(DocumentProperty[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(DocumentProperty[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, DocumentProperty[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;DocumentProperty&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;DocumentProperty&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;DocumentProperty&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;DocumentProperty&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;DocumentProperty&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;DocumentProperty&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;DocumentProperty&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;DocumentProperty&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;DocumentProperty&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;DocumentProperty&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(DocumentProperty) |  |
| [IndexOf](../../aspose.cells.properties/documentpropertycollection/indexof/)(string) | Obtiene el índice de una propiedad por nombre.(Heredado de [`DocumentPropertyCollection`](../documentpropertycollection/).) |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(DocumentProperty, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(DocumentProperty, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(DocumentProperty) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(DocumentProperty, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(DocumentProperty, int, int) |  |
| [Remove](../../aspose.cells.properties/documentpropertycollection/remove/)(string) | Elimina una propiedad con el nombre especificado de la colección.(Heredado de [`DocumentPropertyCollection`](../documentpropertycollection/).) |
| [RemoveAt](../../aspose.cells.properties/documentpropertycollection/removeat/)(int) | Elimina una propiedad en el índice especificado. (2 métodos) |
| [UpdateLinkedPropertyValue](../../aspose.cells.properties/customdocumentpropertycollection/updatelinkedpropertyvalue/)() | Actualiza los valores de todas las propiedades personalizadas que están vinculadas al contenido (utiliza el valor de celda del rango vinculado para actualizar el valor de la propiedad personalizada). |
| [UpdateLinkedRange](../../aspose.cells.properties/customdocumentpropertycollection/updatelinkedrange/)() | Actualiza todos los rangos que están vinculados a propiedades personalizadas (utiliza el valor de la propiedad de documento personalizada para actualizar el valor de celda del rango vinculado). |

### Observaciones

Cada objeto [`DocumentProperty`](../documentproperty/) representa una propiedad personalizada de un documento contenedor.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Properties;
    using System;

    public class CustomDocumentPropertyCollectionDemo
    {
        public static void CustomDocumentPropertyCollectionExample()
        {
            // Instanciar un objeto Workbook
            Workbook workbook = new Workbook();

            // Recuperar una lista de todas las propiedades de documento personalizadas del archivo Excel
            CustomDocumentPropertyCollection customProperties = workbook.Worksheets.CustomDocumentProperties;

            // Agregar propiedades de documento personalizadas
            customProperties.Add("Author", "John Doe");
            customProperties.Add("Revision", 3);
            customProperties.Add("LastModified", DateTime.Now);
            customProperties.Add("IsFinal", true);
            customProperties.Add("Rating", 4.5);

            // Agregar una propiedad de documento personalizada vinculada
            customProperties.AddLinkToContent("LinkedProperty", "Sheet1!A1");

            // Actualizar valores de propiedades vinculadas
            //customProperties.UpdateLinkedPropertyValue();
            customProperties.UpdateLinkedRange();

            // Accediendo a propiedades de documento personalizadas
            DocumentProperty authorProperty = customProperties["Author"];
            DocumentProperty revisionProperty = customProperties["Revision"];
            DocumentProperty lastModifiedProperty = customProperties["LastModified"];
            DocumentProperty isFinalProperty = customProperties["IsFinal"];
            DocumentProperty ratingProperty = customProperties["Rating"];
            DocumentProperty linkedProperty = customProperties["LinkedProperty"];

            // Imprimir propiedades de documento personalizadas
            Console.WriteLine($"Author: {authorProperty.Value}");
            Console.WriteLine($"Revision: {revisionProperty.ToInt()}");
            Console.WriteLine($"Last Modified: {lastModifiedProperty.ToDateTime()}");
            Console.WriteLine($"Is Final: {isFinalProperty.ToBool()}");
            Console.WriteLine($"Rating: {ratingProperty.ToDouble()}");
            Console.WriteLine($"Linked Property: {linkedProperty.Value}");

            // Guarda el libro de trabajo
            workbook.Save("CustomDocumentPropertiesExample.xlsx");
            workbook.Save("CustomDocumentPropertiesExample.pdf");
        }
    }
}
```

### Ver también

* class [DocumentPropertyCollection](../documentpropertycollection/)
* namespace [Aspose.Cells.Properties](../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../)


