---
title: "Classe ValidationCollection"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.ValidationCollection. Représente une collection de validation de données"
type: docs
url: /fr/net/aspose.cells/validationcollection/
---
## ValidationCollection class

Représente la collection de validation des données.

```csharp
public class ValidationCollection : CollectionBase<Validation>
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells/validationcollection/item/) { get; } | Obtient l'élément [`Validation`](../validation/) à l'index spécifié. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Méthodes

| Nom | Description |
| --- | --- |
| [Add](../../aspose.cells/validationcollection/add/#add)() | (**Obsolete.**) Ajoute une validation de données à la collection. |
| [Add](../../aspose.cells/validationcollection/add/#add_1)(CellArea) | Ajoute une validation de données à la collection. |
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
| [GetValidationInCell](../../aspose.cells/validationcollection/getvalidationincell/)(int, int) | Obtient la validation appliquée à la cellule donnée. |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Validation) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Validation, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Validation, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Validation) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Validation, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Validation, int, int) |  |
| [RemoveACell](../../aspose.cells/validationcollection/removeacell/)(int, int) | Supprime tous les paramètres de validation sur la cellule. |
| [RemoveArea](../../aspose.cells/validationcollection/removearea/)(CellArea) | Supprime tous les paramètres de validation sur la plage. |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ValidationCollectionDemo
    {
        public static void ValidationCollectionExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            // Accédez à la collection de validation de la feuille de calcul
            ValidationCollection validations = worksheet.Validations;

            // Définissez une zone de cellules pour la validation
            CellArea area = CellArea.CreateCellArea(0, 0, 1, 1);

            // Ajoutez une validation à la collection
            int validationIndex = validations.Add(area);
            Validation validation = validations[validationIndex];

            // Définir les propriétés de validation
            validation.Type = ValidationType.List;
            validation.Formula1 = "a,b,c,d";

            // Enregistrez le classeur
            workbook.Save("ValidationCollectionExample.xlsx");

            return;
        }
    }
}
```

### Voir aussi

* class [CollectionBase&lt;T&gt;](../collectionbase-1/)
* class [Validation](../validation/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


