---
title: "Class ErrorCheckOptionCollection"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.ErrorCheckOptionCollection classe. Représente toutes les options de vérification d'erreurs"
type: docs
url: /fr/net/aspose.cells/errorcheckoptioncollection/
---
## ErrorCheckOptionCollection class

Représente toutes les options de vérification d'erreurs.

```csharp
public class ErrorCheckOptionCollection : CollectionBase<ErrorCheckOption>
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells/errorcheckoptioncollection/item/) { get; } | Obtient l'objet [`ErrorCheckOption`](../errorcheckoption/) par l'index donné. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Méthodes

| Nom | Description |
| --- | --- |
| [Add](../../aspose.cells/errorcheckoptioncollection/add/)() | Ajoutez une option de vérification d'erreurs. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(ErrorCheckOption) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(ErrorCheckOption, IComparer&lt;ErrorCheckOption&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, ErrorCheckOption, IComparer&lt;ErrorCheckOption&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(ErrorCheckOption) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(ErrorCheckOption[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(ErrorCheckOption[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, ErrorCheckOption[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;ErrorCheckOption&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;ErrorCheckOption&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;ErrorCheckOption&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;ErrorCheckOption&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;ErrorCheckOption&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;ErrorCheckOption&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;ErrorCheckOption&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;ErrorCheckOption&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;ErrorCheckOption&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;ErrorCheckOption&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(ErrorCheckOption) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(ErrorCheckOption, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(ErrorCheckOption, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(ErrorCheckOption) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(ErrorCheckOption, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(ErrorCheckOption, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassErrorCheckOptionCollectionDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            ErrorCheckOptionCollection errorCheckOptions = worksheet.ErrorCheckOptions;
            int optionIndex = errorCheckOptions.Add();
            ErrorCheckOption errorCheckOption = errorCheckOptions[optionIndex];

            errorCheckOption.SetErrorCheck(ErrorCheckType.InconsistFormula, false);
            errorCheckOption.SetErrorCheck(ErrorCheckType.TextNumber, false);

            CellArea cellArea = CellArea.CreateCellArea("A1", "C5");
            errorCheckOption.AddRange(cellArea);

            workbook.Save("ErrorCheckOptionsDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [CollectionBase&lt;T&gt;](../collectionbase-1/)
* class [ErrorCheckOption](../errorcheckoption/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


