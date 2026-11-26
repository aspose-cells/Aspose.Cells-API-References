---
title: "Clase ValidationCollection"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.ValidationCollection. Representa una colección de validación de datos"
type: docs
url: /es/net/aspose.cells/validationcollection/
---
## ValidationCollection class

Representa la colección de validación de datos.

```csharp
public class ValidationCollection : CollectionBase<Validation>
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells/validationcollection/item/) { get; } | Obtiene el elemento [`Validation`](../validation/) en el índice especificado. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [Add](../../aspose.cells/validationcollection/add/#add)() | (**Obsolete.**) Agrega una validación de datos a la colección. |
| [Add](../../aspose.cells/validationcollection/add/#add_1)(CellArea) | Agrega una validación de datos a la colección. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(Validation) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(Validation, IComparer&lt;Validation&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, Validation, IComparer&lt;Validation&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(Validation) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(Validation[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(Validation[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, Validation[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;Validation&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;Validation&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;Validation&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;Validation&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;Validation&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;Validation&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;Validation&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;Validation&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;Validation&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;Validation&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [GetValidationInCell](../../aspose.cells/validationcollection/getvalidationincell/)(int, int) | Obtiene la validación aplicada a la celda dada. |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Validation) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Validation, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Validation, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Validation) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Validation, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Validation, int, int) |  |
| [RemoveACell](../../aspose.cells/validationcollection/removeacell/)(int, int) | Elimina todas las configuraciones de validación en la celda. |
| [RemoveArea](../../aspose.cells/validationcollection/removearea/)(CellArea) | Elimina todas las configuraciones de validación en el rango.. |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ValidationCollectionDemo
    {
        public static void ValidationCollectionExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            // Accede a la colección de validación de la hoja de cálculo
            ValidationCollection validations = worksheet.Validations;

            // Defina un área de celdas para la validación
            CellArea area = CellArea.CreateCellArea(0, 0, 1, 1);

            // Agrega una validación a la colección
            int validationIndex = validations.Add(area);
            Validation validation = validations[validationIndex];

            // Establezca propiedades de validación
            validation.Type = ValidationType.List;
            validation.Formula1 = "a,b,c,d";

            // Guarda el libro de trabajo
            workbook.Save("ValidationCollectionExample.xlsx");

            return;
        }
    }
}
```

### Ver también

* class [CollectionBase&lt;T&gt;](../collectionbase-1/)
* class [Validation](../validation/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


