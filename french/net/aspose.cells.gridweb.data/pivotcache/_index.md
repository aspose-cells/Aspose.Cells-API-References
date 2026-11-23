---
title: "Classe PivotCache"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.GridWeb.Data.PivotCache. Représente le cache mémoire pour un rapport PivotTable. L'objet PivotCache est un membre de la collection PivotCaches"
type: docs
url: /fr/net/aspose.cells.gridweb.data/pivotcache/
---
## PivotCache class

Représente le cache mémoire pour un rapport PivotTable. L'objet PivotCache est un membre de la collection [`PivotCaches`](../pivotcaches/).

```csharp
[Obsolete("This class is obsolete; use GridPivotTable instead")]
public class PivotCache
```

## Propriétés

| Nom | Description |
| --- | --- |
| [DataTable](../../aspose.cells.gridweb.data/pivotcache/datatable/) { get; } | Renvoie la source de données de System.Data.DataTable pour le rapport PivotTable. |
| [DataView](../../aspose.cells.gridweb.data/pivotcache/dataview/) { get; } | Renvoie la source de données de System.Data.DataView pour le rapport PivotTable. |
| [Index](../../aspose.cells.gridweb.data/pivotcache/index/) { get; } | Renvoie l'index de cet objet dans le Parent |
| [Name](../../aspose.cells.gridweb.data/pivotcache/name/) { get; } | Renvoie le nom de PivotCache.Re |
| [Parent](../../aspose.cells.gridweb.data/pivotcache/parent/) { get; } | Renvoie l'objet parent pour l'objet spécifié (le conteneur de PivotCache). Lecture seule. |
| [SourceCellArea](../../aspose.cells.gridweb.data/pivotcache/sourcecellarea/) { get; } | Renvoie la plage de la source de données utilisée avec SourceSheet. |
| [SourceSheet](../../aspose.cells.gridweb.data/pivotcache/sourcesheet/) { get; } | Renvoie la source de données de WebWorksheet pour le rapport PivotTable. |
| [SourceType](../../aspose.cells.gridweb.data/pivotcache/sourcetype/) { get; } | Représente le type des données source |

## Méthodes

| Nom | Description |
| --- | --- |
| [CreatePivotTable](../../aspose.cells.gridweb.data/pivotcache/createpivottable/#createpivottable)() | Crée un rapport PivotTable sur une nouvelle feuille. |
| [CreatePivotTable](../../aspose.cells.gridweb.data/pivotcache/createpivottable/#createpivottable_3)(string) | Crée un rapport PivotTable sur une nouvelle feuille. Le nom de l'objet pivotTable |
| [CreatePivotTable](../../aspose.cells.gridweb.data/pivotcache/createpivottable/#createpivottable_1)(WebWorksheet, WebCell) | Crée un rapport PivotTable sur la feuille cible. |
| [CreatePivotTable](../../aspose.cells.gridweb.data/pivotcache/createpivottable/#createpivottable_2)(WebWorksheet, WebCell, string) | Crée un rapport PivotTable sur la feuille cible. |
| override [Equals](../../aspose.cells.gridweb.data/pivotcache/equals/)(object) | Détermine si deux instances d'Object sont égales. |
| override [GetHashCode](../../aspose.cells.gridweb.data/pivotcache/gethashcode/)() | Fait office de fonction de hachage pour un type particulier, adaptée à une utilisation dans les algorithmes de hachage et les structures de données comme une table de hachage. |
| [ResetDataSource](../../aspose.cells.gridweb.data/pivotcache/resetdatasource/#resetdatasource_1)(DataTable) | Réinitialise les données source |
| [ResetDataSource](../../aspose.cells.gridweb.data/pivotcache/resetdatasource/#resetdatasource_2)(DataView) | Réinitialise les données source |
| [ResetDataSource](../../aspose.cells.gridweb.data/pivotcache/resetdatasource/#resetdatasource)(WebWorksheet, WebCellArea) | Réinitialise les données source |
| override [ToString](../../aspose.cells.gridweb.data/pivotcache/tostring/)() | Renvoie une String qui représente l'Object actuel |

### Remarques

NOTE : Cette classe est maintenant obsolète. Veuillez utiliser GridPivotTable à la place. Cette classe sera supprimée après 6 mois à compter d'août 2014. Aspose s'excuse pour tout inconvénient que vous avez pu rencontrer.

Utilise la méthode PivotCache pour renvoyer un objet PivotCache pour un rapport PivotTable (chaque rapport ne possède qu'un seul cache). Les données source de PivotCache proviennent de WebWorksheet, DataTable, etc.

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


