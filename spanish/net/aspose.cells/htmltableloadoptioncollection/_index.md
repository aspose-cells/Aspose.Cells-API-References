---
title: "Clase HtmlTableLoadOptionCollection"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.HtmlTableLoadOptionCollection. Representa las opciones de tabla al importar HTML"
type: docs
url: /es/net/aspose.cells/htmltableloadoptioncollection/
---
## HtmlTableLoadOptionCollection class

Representa las opciones de tabla al importar HTML.

```csharp
public class HtmlTableLoadOptionCollection : CollectionBase<HtmlTableLoadOption>
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [HtmlTableLoadOptionCollection](htmltableloadoptioncollection/)() | El constructor predeterminado. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells/htmltableloadoptioncollection/item/) { get; } | Obtiene el elemento [`HtmlTableLoadOption`](../htmltableloadoption/) en el índice especificado. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |
| [TableToListObject](../../aspose.cells/htmltableloadoptioncollection/tabletolistobject/) { get; set; } | Indica si generar objetos de lista a partir de tablas importadas. El valor predeterminado es false. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [Add](../../aspose.cells/htmltableloadoptioncollection/add/#add)(HtmlTableLoadOption) | (**Obsolete.**) Añade un HtmlTableLoadOption a esta colección. |
| [Add](../../aspose.cells/htmltableloadoptioncollection/add/#add_1)(int) | Agregar un HtmlTableLoadOption a la lista. |
| [Add](../../aspose.cells/htmltableloadoptioncollection/add/#add_4)(string) | Agregar un HtmlTableLoadOption a la lista. |
| [Add](../../aspose.cells/htmltableloadoptioncollection/add/#add_2)(int, int) | Agregar un HtmlTableLoadOption a la lista. |
| [Add](../../aspose.cells/htmltableloadoptioncollection/add/#add_5)(string, int) | Agregar un HtmlTableLoadOption a la lista. |
| [Add](../../aspose.cells/htmltableloadoptioncollection/add/#add_3)(int, int, int) | Agregar un HtmlTableLoadOption a la lista. |
| [Add](../../aspose.cells/htmltableloadoptioncollection/add/#add_6)(string, int, int) | Agregar un HtmlTableLoadOption a la lista. |
| [AddTableLoadOption](../../aspose.cells/htmltableloadoptioncollection/addtableloadoption/)(HtmlTableLoadOption) | Añade un HtmlTableLoadOption a esta colección. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(HtmlTableLoadOption) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(HtmlTableLoadOption, IComparer&lt;HtmlTableLoadOption&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, HtmlTableLoadOption, IComparer&lt;HtmlTableLoadOption&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(HtmlTableLoadOption) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(HtmlTableLoadOption[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(HtmlTableLoadOption[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, HtmlTableLoadOption[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;HtmlTableLoadOption&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;HtmlTableLoadOption&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;HtmlTableLoadOption&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;HtmlTableLoadOption&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;HtmlTableLoadOption&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;HtmlTableLoadOption&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;HtmlTableLoadOption&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;HtmlTableLoadOption&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;HtmlTableLoadOption&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;HtmlTableLoadOption&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(HtmlTableLoadOption) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(HtmlTableLoadOption, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(HtmlTableLoadOption, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(HtmlTableLoadOption) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(HtmlTableLoadOption, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(HtmlTableLoadOption, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class HtmlTableLoadOptionCollectionDemo
    {
        public static void HtmlTableLoadOptionCollectionExample()
        {
            // Crear un nuevo Workbook
            Workbook workbook = new Workbook();

            // Crear HtmlLoadOptions
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();

            // Acceder a la instancia de HtmlTableLoadOptionCollection
            HtmlTableLoadOptionCollection tableLoadOptions = loadOptions.TableLoadOptions;

            // Establecer la propiedad TableToListObject
            tableLoadOptions.TableToListObject = true;

            // Agregar una nueva HtmlTableLoadOption por índice de tabla
            int index1 = tableLoadOptions.Add(0);

            // Agregar una nueva HtmlTableLoadOption por id de tabla
            int index2 = tableLoadOptions.Add("tableId");

            // Agregar una nueva HtmlTableLoadOption por índice de tabla y índice de hoja de destino
            int index3 = tableLoadOptions.Add(1, 1);

            // Agregar una nueva HtmlTableLoadOption por id de tabla y índice de hoja de destino
            int index4 = tableLoadOptions.Add("tableId2", 2);

            // Agregar una nueva HtmlTableLoadOption por índice de tabla, índice de hoja de destino y índice de hoja original
            int index5 = tableLoadOptions.Add(2, 2, 0);

            // Agregar una nueva HtmlTableLoadOption por id de tabla, índice de hoja de destino y índice de hoja original
            int index6 = tableLoadOptions.Add("tableId3", 3, 1);

            // Acceder a la HtmlTableLoadOption en un índice específico
            HtmlTableLoadOption option = tableLoadOptions[index1];

            // Establecer propiedades de la HtmlTableLoadOption
            option.TableIndex = 0;
            option.Id = "tableId";
            option.Name = "TableName";
            option.OriginalSheetIndex = 0;
            option.TargetSheetIndex = 1;
            option.TableToListObject = true;

            // Cargar un archivo HTML en el libro de trabajo usando las opciones de carga
            workbook = new Workbook("HtmlTableLoadOptionCollectionExample_original.html", loadOptions);

            // Guarda el libro de trabajo
            workbook.Save("HtmlTableLoadOptionCollectionExample.xlsx");

            return;
        }
    }
}
```

### Ver también

* class [CollectionBase&lt;T&gt;](../collectionbase-1/)
* class [HtmlTableLoadOption](../htmltableloadoption/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


