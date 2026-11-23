---
title: "Classe PivotAreaCollection"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.Pivot.PivotAreaCollection. Représente une liste de zones pivot"
type: docs
url: /fr/net/aspose.cells.pivot/pivotareacollection/
---
## PivotAreaCollection class

Représente une liste de zones de tableau croisé dynamique.

```csharp
public class PivotAreaCollection : CollectionBase<PivotArea>
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.pivot/pivotareacollection/item/) { get; } | Obtient un [`PivotArea`](../pivotarea/) objet; |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Méthodes

| Nom | Description |
| --- | --- |
| [Add](../../aspose.cells.pivot/pivotareacollection/add/#add_1)(CellArea) | Ajoute une zone basée sur la vue du tableau croisé dynamique. |
| [Add](../../aspose.cells.pivot/pivotareacollection/add/#add)(PivotArea) | (**Obsolète.**) Ajoute la zone pivot. |
| [AddPivotArea](../../aspose.cells.pivot/pivotareacollection/addpivotarea/)(PivotArea) | Ajoute la zone pivot à cette collection. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(PivotArea) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(PivotArea, IComparer&lt;PivotArea&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, PivotArea, IComparer&lt;PivotArea&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(PivotArea) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(PivotArea[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(PivotArea[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, PivotArea[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;PivotArea&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;PivotArea&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;PivotArea&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;PivotArea&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;PivotArea&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;PivotArea&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;PivotArea&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;PivotArea&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;PivotArea&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;PivotArea&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(PivotArea) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(PivotArea, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(PivotArea, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(PivotArea) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(PivotArea, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(PivotArea, int, int) |  |
| [RemoveAt](../../aspose.cells.pivot/pivotareacollection/removeat/#removeat)(int) | Supprime un paramètre de zone conditionnelle pivot. (2 méthodes) |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotClassPivotAreaCollectionDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer des données d'exemple pour le tableau croisé dynamique
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("Electronics");
            worksheet.Cells["B2"].PutValue(1500);
            worksheet.Cells["A3"].PutValue("Clothing");
            worksheet.Cells["B3"].PutValue(800);
            worksheet.Cells["A4"].PutValue("Furniture");
            worksheet.Cells["B4"].PutValue(1200);

            // Ajouter un tableau croisé dynamique
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "D3", "SalesPivotTable");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Créer des zones de cellules pour les zones pivot
            CellArea dataArea = new CellArea { StartRow = 1, StartColumn = 1, EndRow = 4, EndColumn = 1 };
            CellArea headerArea = new CellArea { StartRow = 0, StartColumn = 0, EndRow = 0, EndColumn = 1 };

            // Obtenir la collection de zones pivot
            PivotAreaCollection pivotAreas = pivotTable.SelectArea(dataArea);

            // Ajouter des zones pivot
            pivotAreas.Add(dataArea);
            pivotAreas.Add(headerArea);

            // Afficher toutes les zones pivot
            Console.WriteLine("Pivot Areas Count: " + pivotAreas.Count);
            for (int i = 0; i < pivotAreas.Count; i++)
            {
                CellArea[] areas = pivotAreas[i].GetCellAreas();
                foreach (CellArea area in areas)
                {
                    Console.WriteLine($"Area {i}: ({area.StartRow},{area.StartColumn}) to ({area.EndRow},{area.EndColumn})");
                }
            }

            // Supprimer une zone
            pivotAreas.RemoveAt(0);
            Console.WriteLine("\nAfter removal - Pivot Areas Count: " + pivotAreas.Count);

            // Enregistrez le classeur
            workbook.Save("PivotAreaCollectionDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [PivotArea](../pivotarea/)
* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


