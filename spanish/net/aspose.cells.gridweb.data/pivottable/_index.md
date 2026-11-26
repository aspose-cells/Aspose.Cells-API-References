---
title: "Clase PivotTable"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.GridWeb.Data.PivotTable class. Representa un informe PivotTable en una hoja de cálculo. El objeto PivotTable es un miembro de la colección PivotTables. La colección PivotTables contiene todos los objetos PivotTable en un control"
type: docs
url: /es/net/aspose.cells.gridweb.data/pivottable/
---
## PivotTable class

Representa un informe PivotTable en una hoja de cálculo. El objeto PivotTable es un miembro de la colección [`PivotTables`](../pivottables/). La colección PivotTables contiene todos los objetos PivotTable en un control.

```csharp
[Obsolete("This class is obsolete; use GridPivotTable instead")]
public class PivotTable
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Name](../../aspose.cells.gridweb.data/pivottable/name/) { get; } | Obtiene el nombre |
| [PivotCache](../../aspose.cells.gridweb.data/pivottable/pivotcache/) { get; } | Obtiene el objeto PivotCache que utilizó el informe. |
| [PivotFields](../../aspose.cells.gridweb.data/pivottable/pivotfields/) { get; } | Representa todos los campos en el informe PivotTable. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [DataBind](../../aspose.cells.gridweb.data/pivottable/databind/)() |  |

### Observaciones

NOTA: Esta clase está ahora obsoleta. Por favor use GridPivotTable en su lugar. Esta clase será eliminada después de 6 meses desde agosto de 2014. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp

 [C#]

 //Suponiendo que la hoja de cálculo "Sheet1" tiene datos, entonces crea un informe PivotTable basado en ella.
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

 //Crea un informe PivotTable a partir de DataView o DataTable.
 DataView dataView;//Or  DataTable dataTable;
     .
     .
     .
 Sets dataView(dataTable) Value
     .
     .
     .

 PivotCache cache = GridWeb1.WebWorksheets.PivotCaches.Add(dataView);
 //Or PivotCache cache = GridWeb1.WebWorksheets.PivotCaches.Add(dataTable);
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

### Ver también

* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


