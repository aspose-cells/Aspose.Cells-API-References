---
title: TimelineCollection
second_title: Référence de l'API Aspose.Cells pour .NET
description: Spécifie la collection de tous les objets Timeline sur la feuille de calcul spécifiée.
type: docs
weight: 6080
url: /fr/net/aspose.cells.timelines/timelinecollection/
---
## TimelineCollection class

Spécifie la collection de tous les objets Timeline sur la feuille de calcul spécifiée.

```csharp
public class TimelineCollection : CollectionBase<Timeline>
```

## Propriétés

| Nom | La description |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase`1/capacity) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase`1/count) { get; } |  |
| [Item](../../aspose.cells.timelines/timelinecollection/item) { get; } | Obtient la chronologie par index. (2 indexers) |
| [Item](../../aspose.cells/collectionbase`1/item) { get; set; } |  |

## Méthodes

| Nom | La description |
| --- | --- |
| [Add](../../aspose.cells.timelines/timelinecollection/add#add_4)(PivotTable, string, int) | Ajouter une nouvelle chronologie en utilisant le tableau croisé dynamique comme source de données |
| [Add](../../aspose.cells.timelines/timelinecollection/add#add_3)(PivotTable, string, PivotField) | Ajouter une nouvelle chronologie en utilisant le tableau croisé dynamique comme source de données |
| [Add](../../aspose.cells.timelines/timelinecollection/add#add_5)(PivotTable, string, string) | Ajouter une nouvelle chronologie en utilisant le tableau croisé dynamique comme source de données |
| [Add](../../aspose.cells.timelines/timelinecollection/add#add_1)(PivotTable, int, int, int) | Ajouter une nouvelle chronologie en utilisant le tableau croisé dynamique comme source de données |
| [Add](../../aspose.cells.timelines/timelinecollection/add#add)(PivotTable, int, int, PivotField) | Ajouter une nouvelle chronologie en utilisant le tableau croisé dynamique comme source de données |
| [Add](../../aspose.cells.timelines/timelinecollection/add#add_2)(PivotTable, int, int, string) | Ajouter une nouvelle chronologie en utilisant le tableau croisé dynamique comme source de données |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(Timeline) |  |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(Timeline, IComparer&lt;Timeline&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(int, int, Timeline, IComparer&lt;Timeline&gt;) |  |
| [Clear](../../aspose.cells/collectionbase`1/clear)() |  |
| [Contains](../../aspose.cells/collectionbase`1/contains)(Timeline) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(Timeline[]) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(Timeline[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(int, Timeline[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase`1/exists)(Predicate&lt;Timeline&gt;) |  |
| [Find](../../aspose.cells/collectionbase`1/find)(Predicate&lt;Timeline&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase`1/findall)(Predicate&lt;Timeline&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(Predicate&lt;Timeline&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(int, Predicate&lt;Timeline&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(int, int, Predicate&lt;Timeline&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase`1/findlast)(Predicate&lt;Timeline&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(Predicate&lt;Timeline&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(int, Predicate&lt;Timeline&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(int, int, Predicate&lt;Timeline&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase`1/getenumerator)() |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(Timeline) |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(Timeline, int) |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(Timeline, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(Timeline) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(Timeline, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(Timeline, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase`1/removeat)(int) |  |

### Exemples

```csharp

[C#]
Workbook book = new Workbook();
Worksheet sheet = book.Worksheets[0];
Cells cells = sheet.Cells;
cells[0, 0].Value = "fruit";
cells[1, 0].Value = "grape";
cells[2, 0].Value = "blueberry";
cells[3, 0].Value = "kiwi";
cells[4, 0].Value = "cherry";

//Créer un style de date
Style dateStyle = new CellsFactory().CreateStyle();
dateStyle.Custom = "m/d/yyyy";
cells[0, 1].Value = "date";
cells[1, 1].Value = new DateTime(2021, 2, 5);
cells[2, 1].Value = new DateTime(2022, 3, 8);
cells[3, 1].Value = new DateTime(2023, 4, 10);
cells[4, 1].Value = new DateTime(2024, 5, 16);
// Définir le style de date
cells[1, 1].SetStyle(dateStyle);
cells[2, 1].SetStyle(dateStyle);
cells[3, 1].SetStyle(dateStyle);
cells[4, 1].SetStyle(dateStyle);

cells[0, 2].Value = "amount";
cells[1, 2].Value = 50;
cells[2, 2].Value = 60;
cells[3, 2].Value = 70;
cells[4, 2].Value = 80;

PivotTableCollection pivots = sheet.PivotTables;
//Ajouter un tableau croisé dynamique
int pivotIndex = pivots.Add("=Sheet1!A1:C5", "A12", "TestPivotTable");
PivotTable pivot = pivots[pivotIndex];
pivot.AddFieldToArea(PivotFieldType.Row, "fruit");
pivot.AddFieldToArea(PivotFieldType.Column, "date");
pivot.AddFieldToArea(PivotFieldType.Data, "amount");
pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;

// Actualiser les données du tableau croisé dynamique
pivot.RefreshData();
pivot.CalculateData();

//faites vos affaires
book.Save("out.xlsx");

```

### Voir également

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1)
* class [Timeline](../timeline)
* espace de noms [Aspose.Cells.Timelines](../../aspose.cells.timelines)
* Assemblée [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
