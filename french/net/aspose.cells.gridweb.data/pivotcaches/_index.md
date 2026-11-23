---
title: "Classe PivotCaches"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.GridWeb.Data.PivotCaches. Représente la collection de caches mémoire provenant des rapports PivotTable dans un classeur. Chaque cache mémoire est représenté par un objet PivotCache."
type: docs
url: /fr/net/aspose.cells.gridweb.data/pivotcaches/
---
## PivotCaches class

Représente la collection de caches mémoire provenant des rapports PivotTable dans un classeur. Chaque cache mémoire est représenté par un objet [`PivotCache`](../pivotcache/).

```csharp
[Obsolete("This class is obsolete; use GridPivotTableCollection instead")]
public class PivotCaches : ICollection
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Count](../../aspose.cells.gridweb.data/pivotcaches/count/) { get; } | Obtient le nombre d'éléments contenus dans l'instance PivotCaches. |
| [IsSynchronized](../../aspose.cells.gridweb.data/pivotcaches/issynchronized/) { get; } | Obtient une valeur indiquant si l'accès aux PivotCaches est synchronisé (thread-safe). |
| [Item](../../aspose.cells.gridweb.data/pivotcaches/item/) { get; } | Obtient l'objet PivotCache par index. (2 indexeurs) |
| [Parent](../../aspose.cells.gridweb.data/pivotcaches/parent/) { get; } | Obtient l'objet parent pour l'objet spécifié. Lecture seule. |
| [SyncRoot](../../aspose.cells.gridweb.data/pivotcaches/syncroot/) { get; } | Obtient un objet qui peut être utilisé pour synchroniser l'accès aux PivotCaches. |

## Méthodes

| Nom | Description |
| --- | --- |
| [Add](../../aspose.cells.gridweb.data/pivotcaches/add/#add_2)(DataTable) | Ajoute un PivotCache à partir d'un DataTable. |
| [Add](../../aspose.cells.gridweb.data/pivotcaches/add/#add_4)(DataView) | Ajoute un PivotCache à partir d'un DataView. |
| [Add](../../aspose.cells.gridweb.data/pivotcaches/add/#add_3)(DataTable, string) | Ajoute un PivotCahe à partir d'un DataTable en utilisant le nom spécifié. |
| [Add](../../aspose.cells.gridweb.data/pivotcaches/add/#add_5)(DataView, string) | Ajoute un PivotCache à partir d'un DataView en utilisant le nom spécifié. |
| [Add](../../aspose.cells.gridweb.data/pivotcaches/add/#add)(WebWorksheet, WebCellArea) | Ajoute un PivotCache à partir d'une feuille |
| [Add](../../aspose.cells.gridweb.data/pivotcaches/add/#add_1)(WebWorksheet, WebCellArea, string) | Ajoute un PivotCache à partir d'une feuille en utilisant le nom spécifié. |
| [Clear](../../aspose.cells.gridweb.data/pivotcaches/clear/)() | Supprime tous les objets PivotCache et tous les objets PivotTable dans le contrôle. |
| [CopyTo](../../aspose.cells.gridweb.data/pivotcaches/copyto/)(Array, int) | Copie l'intégralité du PivotCache dans un tableau unidimensionnel compatible, en commençant à l'index spécifié du tableau cible. |
| [GetEnumerator](../../aspose.cells.gridweb.data/pivotcaches/getenumerator/)() | Renvoie un IEnumerator pour les PivotCaches. |
| [IndexOf](../../aspose.cells.gridweb.data/pivotcaches/indexof/)(PivotCache) | Renvoie l'index du PivotCache spécifié dans la collection. |
| [Remove](../../aspose.cells.gridweb.data/pivotcaches/remove/)(PivotCache) | Supprime l'objet PivotCache spécifié des PivotCaches ainsi que le PivotTable associé en utilisant le pivotCache comme source de données. |
| [RemoveAt](../../aspose.cells.gridweb.data/pivotcaches/removeat/)(int) | Supprime l'objet PivotCache spécifié des PivotCaches ainsi que le PivotTable associé en utilisant le pivotCache comme source de données. |

### Remarques

NOTE : Cette classe est maintenant obsolète. Veuillez utiliser GridPivotTableCollection à la place. Cette classe sera supprimée après 6 mois à compter d'août 2014. Aspose s'excuse pour tout inconvénient que vous auriez pu rencontrer.

### Exemples

```csharp

 [C#]

 //En supposant que la feuille de calcul "Sheet1" contient des données, crée alors un rapport PivotTable basé sur celle‑ci.
 WebWorksheet sourceSheet = GridWeb1.WebWorksheets["Sheet1"];
 Aspose.Cells.GridWeb.Data.WebCellArea sourceRange = new WebCellArea();
 sourceRange.StartRow = 0;
 sourceRange.StartColumn = 0;
 sourceRange.EndRow = 10;
 sourceRange.EndColumn = 5;

 PivotCache cache = GridWeb1.WebWorksheets.PivotCaches.Add(sourceSheet, sourceRange);

 PivotTable table = cache.CreatePivotTable();

 table.PivotFields[0].Orientation = PivotFieldOrientation.RowField;
 table.PivotFields[1].Orientation = PivotFieldOrientation.RowField;
 table.PivotFields[2].Orientation = PivotFieldOrientation.RowField;
 table.PivotFields[3].Orientation = PivotFieldOrientation.ColumnField | PivotFieldOrientation.DataField;
 table.PivotFields[4].Orientation = PivotFieldOrientation.ColumnField;
 table.PivotFields[5].Orientation = PivotFieldOrientation.ColumnField | PivotFieldOrientation.DataField;

 table.PivotFields[3].Function = PivotFieldFunction.Count;
 table.PivotFields[5].Function = PivotFieldFunction.Sum;

 table.DataBind();

 //Crée un rapport PivotTable à partir de DataView ou DataTable.
 DataView dataView;//Or  DataTable dataTable;
     .
     .
     .
 Sets dataView(dataTable) Value
     .
     .
     .

 PivotCache cache = GridWeb1.WebWorksheets.PivotCaches.Add(dataView);
 //Ou `PivotCache cache = GridWeb1.WebWorksheets.PivotCaches.Add(dataTable);`
 PivotTable table = cache.CreatePivotTable();
 table = GridWeb1.WebWorksheets.PivotTables["PivotTable1"];
 table.PivotFields[0].Orientation = PivotFieldOrientation.RowField;
 table.PivotFields[1].Orientation = PivotFieldOrientation.RowField;
 table.PivotFields[2].Orientation = PivotFieldOrientation.ColumnField | PivotFieldOrientation.DataField;
 table.DataBind();


 [VB]


 'On the assumption that worksheet "Sheet1" has datas, then creates a PivotTable report base on it.
 Dim sourceSheet As WebWorksheet =  GridWeb1.WebWorksheets("Sheet1")
 Dim sourceRange As Aspose.Cells.GridWeb.Data.WebCellArea =  New WebCellArea()/
 sourceRange.StartRow = 0
 sourceRange.StartColumn = 0
 sourceRange.EndRow = 10
 sourceRange.EndColumn = 5

 Dim cache As PivotCache =  GridWeb1.WebWorksheets.PivotCaches.Add(sourceSheet,sourceRange)

 Dim table As PivotTable =  cache.CreatePivotTable()

 table.PivotFields(0).Orientation = PivotFieldOrientation.RowField
 table.PivotFields(1).Orientation = PivotFieldOrientation.RowField
 table.PivotFields(2).Orientation = PivotFieldOrientation.RowField
 table.PivotFields(3).Orientation = PivotFieldOrientation.ColumnField | PivotFieldOrientation.DataField
 table.PivotFields(4).Orientation = PivotFieldOrientation.ColumnField
 table.PivotFields(5).Orientation = PivotFieldOrientation.ColumnField | PivotFieldOrientation.DataField

 table.PivotFields(3).Function = PivotFieldFunction.Count
 table.PivotFields(5).Function = PivotFieldFunction.Sum

 table.DataBind()

 'Creates a PivotTable report from DataView or DataTable.

 Dim dataView As DataView ' Or Dim dataTable As DataTable
     .
     .
 Sets dataView(dataTable) Value
     .
     .
     .

 Dim cache As PivotCache =  GridWeb1.WebWorksheets.PivotCaches.Add(dataView)
 'Or Dim cache As PivotCache =  GridWeb1.WebWorksheets.PivotCaches.Add(dataTable)
 Dim table As PivotTable =  cache.CreatePivotTable()
 table = GridWeb1.WebWorksheets.PivotTables("PivotTable1")
 table.PivotFields(0).Orientation = PivotFieldOrientation.RowField
 table.PivotFields(1).Orientation = PivotFieldOrientation.RowField
 table.PivotFields(2).Orientation = PivotFieldOrientation.ColumnField | PivotFieldOrientation.DataField
 table.DataBind()

```

### Voir aussi

* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


