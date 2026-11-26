---
title: "Clase XmlMapCollection"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.XmlMapCollection. Una colección de objetos XmlMap que representan información de XmlMap"
type: docs
url: /es/net/aspose.cells/xmlmapcollection/
---
## XmlMapCollection class

Una colección de [`XmlMap`](../xmlmap/) objetos que representan información de XmlMap.

```csharp
public class XmlMapCollection : CollectionBase<XmlMap>
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells/xmlmapcollection/item/) { get; } | Obtiene el mapa xml por el índice específico. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [Add](../../aspose.cells/xmlmapcollection/add/)(string) | Agrega un [`XmlMap`](../xmlmap/) mediante la url/ruta de un archivo xml/xsd. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(XmlMap) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(XmlMap, IComparer&lt;XmlMap&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, XmlMap, IComparer&lt;XmlMap&gt;) |  |
| [Clear](../../aspose.cells/xmlmapcollection/clear/#clear)() | Elimina todos los XmlMaps. (2 métodos) |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(XmlMap) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(XmlMap[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(XmlMap[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, XmlMap[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;XmlMap&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;XmlMap&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;XmlMap&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;XmlMap&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;XmlMap&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;XmlMap&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;XmlMap&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;XmlMap&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;XmlMap&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;XmlMap&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(XmlMap) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(XmlMap, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(XmlMap, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(XmlMap) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(XmlMap, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(XmlMap, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class XmlMapCollectionDemo
    {
        public static void XmlMapCollectionExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Acceda a XmlMapCollection desde el libro de trabajo
            XmlMapCollection xmlMaps = workbook.Worksheets.XmlMaps;

            // Agregue un nuevo XmlMap a la colección
            int xmlMapIndex = xmlMaps.Add("sample.xml");

            // Acceda al XmlMap recién agregado
            XmlMap xmlMap = xmlMaps[xmlMapIndex];

            // Muestre el recuento de XmlMaps en la colección
            Console.WriteLine("Number of XmlMaps: " + xmlMaps.Count);

            // Establezca la capacidad de XmlMapCollection
            xmlMaps.Capacity = 10;

            // Borre todos los XmlMaps de la colección
            xmlMaps.Clear();

            // Guarda el libro de trabajo
            workbook.Save("XmlMapCollectionExample.xlsx");

            return;
        }
    }
}
```

### Ver también

* class [CollectionBase&lt;T&gt;](../collectionbase-1/)
* class [XmlMap](../xmlmap/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


