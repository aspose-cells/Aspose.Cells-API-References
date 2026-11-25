---
title: "Classe ValidationCollection"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.ValidationCollection. Rappresenta la raccolta di convalida dei dati"
type: docs
url: /it/net/aspose.cells/validationcollection/
---
## ValidationCollection class

Rappresenta la raccolta di convalide dei dati.

```csharp
public class ValidationCollection : CollectionBase<Validation>
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells/validationcollection/item/) { get; } | Ottiene l'elemento [`Validation`](../validation/) all'indice specificato. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Add](../../aspose.cells/validationcollection/add/#add)() | (**Obsolete.**) Aggiunge una convalida dei dati alla raccolta. |
| [Add](../../aspose.cells/validationcollection/add/#add_1)(CellArea) | Aggiunge una convalida dei dati alla raccolta. |
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
| [GetValidationInCell](../../aspose.cells/validationcollection/getvalidationincell/)(int, int) | Ottiene la convalida applicata alla cella specificata. |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Validation) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Validation, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Validation, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Validation) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Validation, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Validation, int, int) |  |
| [RemoveACell](../../aspose.cells/validationcollection/removeacell/)(int, int) | Rimuove tutte le impostazioni di convalida sulla cella. |
| [RemoveArea](../../aspose.cells/validationcollection/removearea/)(CellArea) | Rimuove tutte le impostazioni di convalida sull'intervallo.. |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ValidationCollectionDemo
    {
        public static void ValidationCollectionExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            // Accedi alla raccolta di convalida del foglio di lavoro
            ValidationCollection validations = worksheet.Validations;

            // Definisci un'area di celle per la convalida
            CellArea area = CellArea.CreateCellArea(0, 0, 1, 1);

            // Aggiungi una convalida alla raccolta
            int validationIndex = validations.Add(area);
            Validation validation = validations[validationIndex];

            // Imposta le proprietà di convalida
            validation.Type = ValidationType.List;
            validation.Formula1 = "a,b,c,d";

            // Salva la cartella di lavoro
            workbook.Save("ValidationCollectionExample.xlsx");

            return;
        }
    }
}
```

### Vedi anche

* class [CollectionBase&lt;T&gt;](../collectionbase-1/)
* class [Validation](../validation/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


