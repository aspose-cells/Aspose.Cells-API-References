---
title: "Clase NameCollection"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.NameCollection. Representa una colección de todos los objetos Name en la hoja de cálculo"
type: docs
url: /es/net/aspose.cells/namecollection/
---
## NameCollection class

Representa una colección de todos los objetos [`Name`](../name/) en la hoja de cálculo.

```csharp
public class NameCollection : CollectionBase<Name>
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells/namecollection/item/) { get; } | Obtiene el elemento [`Name`](../name/) en el índice especificado. (2 indexadores) |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [Add](../../aspose.cells/namecollection/add/)(string) | Define un nuevo nombre. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(Name) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(Name, IComparer&lt;Name&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, Name, IComparer&lt;Name&gt;) |  |
| [Clear](../../aspose.cells/namecollection/clear/#clear)() | Elimina todos los nombres definidos que no están referenciados por las fórmulas y la fuente de datos. Si el nombre definido está referenciado, solo establecemos Name.ReferTo como null y los ocultamos. (2 métodos) |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(Name) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(Name[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(Name[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, Name[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;Name&gt;) |  |
| [Filter](../../aspose.cells/namecollection/filter/)(NameScopeType, int) | Obtiene todos los nombres definidos por ámbito. |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;Name&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;Name&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;Name&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;Name&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;Name&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;Name&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;Name&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;Name&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;Name&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Name) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Name, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Name, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Name) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Name, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Name, int, int) |  |
| [Remove](../../aspose.cells/namecollection/remove/#remove)(string) | Eliminar el nombre. |
| [Remove](../../aspose.cells/namecollection/remove/#remove_1)(string[]) | Eliminar una matriz de nombres |
| [RemoveAt](../../aspose.cells/namecollection/removeat/#removeat)(int) | Eliminar el nombre en el índice específico. (2 métodos) |
| [RemoveDuplicateNames](../../aspose.cells/namecollection/removeduplicatenames/)() | Eliminar los nombres definidos duplicados |
| [Sort](../../aspose.cells/namecollection/sort/)() | Ordena los nombres definidos. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class NameCollectionDemo
    {
        public static void NameCollectionExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la colección de hojas de cálculo
            WorksheetCollection worksheets = workbook.Worksheets;
            
            // Acceder a la colección de nombres
            NameCollection names = worksheets.Names;
            
            // Agregar un nuevo nombre a la colección
            int nameIndex = names.Add("MyNamedRange");
            Name name = names[nameIndex];
            
            // Establecer la propiedad refers to para el nombre
            name.RefersTo = "=Sheet1!$A$1:$A$10";
            
            // Acceder y modificar las propiedades del nombre
            name.Comment = "This is a named range for demonstration.";
            name.IsVisible = true;
            
            // Agregar otro nombre
            int anotherNameIndex = names.Add("AnotherNamedRange");
            Name anotherName = names[anotherNameIndex];
            anotherName.RefersTo = "=Sheet1!$B$1:$B$10";
            
            // Eliminar un nombre por texto
            names.Remove("AnotherNamedRange");
            
            // Eliminar un nombre por índice
            names.RemoveAt(nameIndex);
            
            // Borrar todos los nombres
            names.Clear();
            
            // Guarda el libro de trabajo
            workbook.Save("NameCollectionExample.xlsx");

            return;
        }
    }
}
```

### Ver también

* class [CollectionBase&lt;T&gt;](../collectionbase-1/)
* class [Name](../name/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


