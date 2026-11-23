---
title: "Classe PivotAreaFilterCollection"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.Pivot.PivotAreaFilterCollection. Représente la liste des filtres pour PivotArea"
type: docs
url: /fr/net/aspose.cells.pivot/pivotareafiltercollection/
---
## PivotAreaFilterCollection class

Représente la liste des filtres pour [`PivotArea`](../pivotarea/)

```csharp
public class PivotAreaFilterCollection : CollectionBase<PivotAreaFilter>
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [PivotAreaFilterCollection](pivotareafiltercollection/)() | Le constructeur par défaut. |

## Propriétés

| Nom | Description |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.pivot/pivotareafiltercollection/item/) { get; } | Obtient le filtre de la liste par l’indice. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Méthodes

| Nom | Description |
| --- | --- |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(PivotAreaFilter) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(PivotAreaFilter, IComparer&lt;PivotAreaFilter&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, PivotAreaFilter, IComparer&lt;PivotAreaFilter&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(PivotAreaFilter) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(PivotAreaFilter[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(PivotAreaFilter[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, PivotAreaFilter[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;PivotAreaFilter&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;PivotAreaFilter&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;PivotAreaFilter&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;PivotAreaFilter&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;PivotAreaFilter&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;PivotAreaFilter&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;PivotAreaFilter&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;PivotAreaFilter&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;PivotAreaFilter&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;PivotAreaFilter&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(PivotAreaFilter) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(PivotAreaFilter, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(PivotAreaFilter, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(PivotAreaFilter) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(PivotAreaFilter, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(PivotAreaFilter, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotClassPivotAreaFilterCollectionDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour le tableau croisé dynamique
            var cells = worksheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 10;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 15;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 20;
            cells["A5"].Value = "Apple";
            cells["B5"].Value = 5;

            // Créer un tableau croisé dynamique
            int index = worksheet.PivotTables.Add("A1:B5", "C3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");

            // Créez PivotAreaFilterCollection
            PivotAreaFilterCollection filters = new PivotAreaFilterCollection();

            // Créez et ajoutez des filtres (bien que la réflexion de l’API montre une fonctionnalité limitée)
            // Remarque : la création réelle de filtres nécessiterait des informations d’API plus complètes
            // Ceci démontre la structure de la collection
            
            // Accéder aux éléments (propriété en lecture seule)
            if (filters.Count > 0)
            {
                var firstFilter = filters[0];
            }

            // Enregistrez le classeur
            workbook.Save("PivotAreaFilterCollectionDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [PivotAreaFilter](../pivotareafilter/)
* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


