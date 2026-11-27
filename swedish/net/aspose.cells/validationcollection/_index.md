---
title: "Klass ValidationCollection"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.ValidationCollection-klass. Representerar samling för datavalidering"
type: docs
url: /sv/net/aspose.cells/validationcollection/
---
## ValidationCollection class

Representerar samlingen för datavalidering.

```csharp
public class ValidationCollection : CollectionBase<Validation>
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells/validationcollection/item/) { get; } | Hämtar [`Validation`](../validation/) elementet på det angivna indexet. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [Add](../../aspose.cells/validationcollection/add/#add)() | (**Obsolete.**) Lägger till en datavalidering i samlingen. |
| [Add](../../aspose.cells/validationcollection/add/#add_1)(CellArea) | Lägger till en datavalidering i samlingen. |
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
| [GetValidationInCell](../../aspose.cells/validationcollection/getvalidationincell/)(int, int) | Hämtar valideringen som tillämpas på den angivna cellen. |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Validation) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Validation, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Validation, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Validation) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Validation, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Validation, int, int) |  |
| [RemoveACell](../../aspose.cells/validationcollection/removeacell/)(int, int) | Tar bort alla valideringsinställningar på cellen. |
| [RemoveArea](../../aspose.cells/validationcollection/removearea/)(CellArea) | Tar bort alla valideringsinställningar på området.. |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ValidationCollectionDemo
    {
        public static void ValidationCollectionExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            // Åtkomst till valideringssamlingen för kalkylbladet
            ValidationCollection validations = worksheet.Validations;

            // Definiera ett cellområde för valideringen
            CellArea area = CellArea.CreateCellArea(0, 0, 1, 1);

            // Lägg till en validering i samlingen
            int validationIndex = validations.Add(area);
            Validation validation = validations[validationIndex];

            // Ställ in valideringsegenskaper
            validation.Type = ValidationType.List;
            validation.Formula1 = "a,b,c,d";

            // Spara arbetsboken
            workbook.Save("ValidationCollectionExample.xlsx");

            return;
        }
    }
}
```

### Se även

* class [CollectionBase&lt;T&gt;](../collectionbase-1/)
* class [Validation](../validation/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


