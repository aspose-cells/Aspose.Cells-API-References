---
title: "Classe PivotTables"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.GridWeb.Data.PivotTables. Représente une collection de tous les objets PivotTable."
type: docs
url: /fr/net/aspose.cells.gridweb.data/pivottables/
---
## PivotTables class

Représente une collection de tous les objets [`PivotTable`](../pivottable/).

```csharp
[Obsolete("This class is obsolete; use GridPivotTableCollection instead")]
public class PivotTables : ICollection
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Count](../../aspose.cells.gridweb.data/pivottables/count/) { get; } | Obtient le nombre d'éléments contenus dans l'instance PivotTables. |
| [IsSynchronized](../../aspose.cells.gridweb.data/pivottables/issynchronized/) { get; } | Obtient une valeur indiquant si l'accès aux PivotTables est synchronisé (thread-safe). |
| [Item](../../aspose.cells.gridweb.data/pivottables/item/) { get; } | Obtient un objet PivotTable par index. (2 indexeurs) |
| [Parent](../../aspose.cells.gridweb.data/pivottables/parent/) { get; } | Obtient l'objet parent pour l'objet spécifié. Lecture seule. |
| [SyncRoot](../../aspose.cells.gridweb.data/pivottables/syncroot/) { get; } | Obtient un objet pouvant être utilisé pour synchroniser l'accès aux PivotTables. |

## Méthodes

| Nom | Description |
| --- | --- |
| [Add](../../aspose.cells.gridweb.data/pivottables/add/#add)(PivotCache) | Ajoute un objet PivotTable du PivotCache spécifié à une nouvelle feuille de calcul. |
| [Add](../../aspose.cells.gridweb.data/pivottables/add/#add_3)(PivotCache, string) | Ajoute un objet PivotTable du PivotCache spécifié à une nouvelle feuille de calcul. |
| [Add](../../aspose.cells.gridweb.data/pivottables/add/#add_1)(PivotCache, WebWorksheet, WebCell) | Ajoute un objet PivotTable du PivotCache spécifié à la feuille de calcul spécifiée. |
| [Add](../../aspose.cells.gridweb.data/pivottables/add/#add_2)(PivotCache, WebWorksheet, WebCell, string) | Ajoute un objet PivotTable du PivotCache spécifié à la feuille de calcul spécifiée. |
| [Clear](../../aspose.cells.gridweb.data/pivottables/clear/)() | Supprime tous les objets PivotTable et tous les objets PivotCache du contrôle. |
| [Contains](../../aspose.cells.gridweb.data/pivottables/contains/)(string) | Renvoie true si le nom de pivottable tableName existe. |
| [CopyTo](../../aspose.cells.gridweb.data/pivottables/copyto/)(Array, int) | Copie l'intégralité du PivotTable dans un tableau unidimensionnel compatible, en commençant à l'index spécifié du tableau cible |
| [GetEnumerator](../../aspose.cells.gridweb.data/pivottables/getenumerator/)() | Renvoie un IEnumerator pour les PivotTables. |
| [Refresh](../../aspose.cells.gridweb.data/pivottables/refresh/)(PivotTable) | ReDataBinds la source de données au rapport PivotTable. |
| [RefreshAll](../../aspose.cells.gridweb.data/pivottables/refreshall/)() | ReDataBinds la source de données à tous les rapports PivotTable. |
| [Remove](../../aspose.cells.gridweb.data/pivottables/remove/)(PivotTable) | Supprime l'objet PivotTable spécifié des PivotTables et du PivotCache associé s'il n'est pas utilisé par un autre PivotTable. |
| [RemoveAt](../../aspose.cells.gridweb.data/pivottables/removeat/)(int) | Supprime l'objet PivotTable spécifié des PivotTables et du PivotCache associé s'il n'est pas utilisé par un autre PivotTable. |

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


