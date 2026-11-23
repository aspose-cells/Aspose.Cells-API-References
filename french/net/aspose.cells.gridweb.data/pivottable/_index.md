---
title: "Classe PivotTable"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.GridWeb.Data.PivotTable. Représente un rapport PivotTable sur une feuille de calcul. L'objet PivotTable est un membre de la collection PivotTables. La collection PivotTables contient tous les objets PivotTable d'un contrôle."
type: docs
url: /fr/net/aspose.cells.gridweb.data/pivottable/
---
## PivotTable class

Représente un rapport PivotTable sur une feuille de calcul. L'objet PivotTable est un membre de la collection [`PivotTables`](../pivottables/). La collection PivotTables contient tous les objets PivotTable d'un contrôle.

```csharp
[Obsolete("This class is obsolete; use GridPivotTable instead")]
public class PivotTable
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Name](../../aspose.cells.gridweb.data/pivottable/name/) { get; } | Obtient le nom |
| [PivotCache](../../aspose.cells.gridweb.data/pivottable/pivotcache/) { get; } | Obtient l'objet PivotCache utilisé par le rapport. |
| [PivotFields](../../aspose.cells.gridweb.data/pivottable/pivotfields/) { get; } | Représente tous les champs du rapport PivotTable. |

## Méthodes

| Nom | Description |
| --- | --- |
| [DataBind](../../aspose.cells.gridweb.data/pivottable/databind/)() |  |

### Remarques

NOTE : Cette classe est maintenant obsolète. Veuillez utiliser GridPivotTable à la place. Cette classe sera supprimée après 6 mois à compter d'août 2014. Aspose s'excuse pour tout inconvénient que vous avez pu rencontrer.

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


