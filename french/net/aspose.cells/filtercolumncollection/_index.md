---
title: "Classe FilterColumnCollection"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.FilterColumnCollection. Une collection d'objets Filter qui représente tous les filtres d'une plage autofiltée"
type: docs
url: /fr/net/aspose.cells/filtercolumncollection/
---
## FilterColumnCollection class

Une collection d'objets Filter qui représente tous les filtres dans une plage autofiltrée.

```csharp
public class FilterColumnCollection : CollectionBase<FilterColumn>
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells/filtercolumncollection/item/) { get; } | Obtient l'objet [`FilterColumn`](../filtercolumn/) au champ spécial. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Méthodes

| Nom | Description |
| --- | --- |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(FilterColumn) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(FilterColumn, IComparer&lt;FilterColumn&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, FilterColumn, IComparer&lt;FilterColumn&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(FilterColumn) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(FilterColumn[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(FilterColumn[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, FilterColumn[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;FilterColumn&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;FilterColumn&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;FilterColumn&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;FilterColumn&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;FilterColumn&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;FilterColumn&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;FilterColumn&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;FilterColumn&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;FilterColumn&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;FilterColumn&gt;) |  |
| [GetByIndex](../../aspose.cells/filtercolumncollection/getbyindex/)(int) | Renvoie un seul objet Filter d'une collection. |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(FilterColumn) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(FilterColumn, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(FilterColumn, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(FilterColumn) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(FilterColumn, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(FilterColumn, int, int) |  |
| [RemoveAt](../../aspose.cells/filtercolumncollection/removeat/#removeat)(int) | (2 méthodes) |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FilterColumnCollectionDemo
    {
        public static void FilterColumnCollectionExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données au filtre
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(25);
            worksheet.Cells["A3"].PutValue("Jane");
            worksheet.Cells["B3"].PutValue(30);
            worksheet.Cells["A4"].PutValue("Doe");
            worksheet.Cells["B4"].PutValue(22);

            // Créer un AutoFilter
            worksheet.AutoFilter.Range = "A1:B4";

            // Obtenir le FilterColumnCollection
            FilterColumnCollection filterColumns = worksheet.AutoFilter.FilterColumns;

            // Ajouter un filtre à la deuxième colonne (Âge)
            worksheet.AutoFilter.AddFilter(1, "25");

            // Appliquer le filtre
            worksheet.AutoFilter.Refresh();

            // Accéder et manipuler le FilterColumnCollection
            Console.WriteLine("Number of filters applied: " + filterColumns.Count);

            // Obtenir la première colonne de filtre
            FilterColumn filterColumn = filterColumns.GetByIndex(0);
            Console.WriteLine("Filter applied on column index: " + filterColumn.FieldIndex);

            // Supprimer le filtre
            filterColumns.RemoveAt(0);
            worksheet.AutoFilter.Refresh();

            // Enregistrez le classeur
            workbook.Save("FilterColumnCollectionExample.xlsx");
            workbook.Save("FilterColumnCollectionExample.pdf");
        }
    }
}
```

### Voir aussi

* class [CollectionBase&lt;T&gt;](../collectionbase-1/)
* class [FilterColumn](../filtercolumn/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


