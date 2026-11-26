---
title: "Clase PivotCache"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.GridWeb.Data.PivotCache. Representa la caché de memoria para un informe PivotTable. El objeto PivotCache es un miembro de la colección PivotCaches"
type: docs
url: /es/net/aspose.cells.gridweb.data/pivotcache/
---
## PivotCache class

Representa la caché de memoria para un informe PivotTable. El objeto PivotCache es un miembro de la colección [`PivotCaches`](../pivotcaches/).

```csharp
[Obsolete("This class is obsolete; use GridPivotTable instead")]
public class PivotCache
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [DataTable](../../aspose.cells.gridweb.data/pivotcache/datatable/) { get; } | Devuelve la fuente de datos de System.Data.DataTable para el informe PivotTable. |
| [DataView](../../aspose.cells.gridweb.data/pivotcache/dataview/) { get; } | Devuelve la fuente de datos de System.Data.DataView para el informe PivotTable. |
| [Index](../../aspose.cells.gridweb.data/pivotcache/index/) { get; } | Devuelve el índice de este objeto en Parent |
| [Name](../../aspose.cells.gridweb.data/pivotcache/name/) { get; } | Devuelve el nombre de PivotCache.Re |
| [Parent](../../aspose.cells.gridweb.data/pivotcache/parent/) { get; } | Devuelve el objeto padre para el objeto especificado (el contenedor de PivotCache). Solo lectura. |
| [SourceCellArea](../../aspose.cells.gridweb.data/pivotcache/sourcecellarea/) { get; } | Devuelve el rango de la fuente de datos usando SourceSheet. |
| [SourceSheet](../../aspose.cells.gridweb.data/pivotcache/sourcesheet/) { get; } | Devuelve la fuente de datos de WebWorksheet para el informe PivotTable. |
| [SourceType](../../aspose.cells.gridweb.data/pivotcache/sourcetype/) { get; } | Representa el tipo de los datos de origen |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [CreatePivotTable](../../aspose.cells.gridweb.data/pivotcache/createpivottable/#createpivottable)() | Crea un informe PivotTable en una hoja nueva. |
| [CreatePivotTable](../../aspose.cells.gridweb.data/pivotcache/createpivottable/#createpivottable_3)(string) | Crea un informe PivotTable en una hoja nueva. El nombre del objeto pivotTable |
| [CreatePivotTable](../../aspose.cells.gridweb.data/pivotcache/createpivottable/#createpivottable_1)(WebWorksheet, WebCell) | Crea un informe PivotTable en la hoja objetivo. |
| [CreatePivotTable](../../aspose.cells.gridweb.data/pivotcache/createpivottable/#createpivottable_2)(WebWorksheet, WebCell, string) | Crea un informe PivotTable en la hoja objetivo. |
| override [Equals](../../aspose.cells.gridweb.data/pivotcache/equals/)(object) | Determina si dos instancias de Object son iguales. |
| override [GetHashCode](../../aspose.cells.gridweb.data/pivotcache/gethashcode/)() | Funciona como una función hash para un tipo particular, adecuada para su uso en algoritmos de hash y estructuras de datos como una tabla hash. |
| [ResetDataSource](../../aspose.cells.gridweb.data/pivotcache/resetdatasource/#resetdatasource_1)(DataTable) | Restablece los datos de origen |
| [ResetDataSource](../../aspose.cells.gridweb.data/pivotcache/resetdatasource/#resetdatasource_2)(DataView) | Restablece los datos de origen |
| [ResetDataSource](../../aspose.cells.gridweb.data/pivotcache/resetdatasource/#resetdatasource)(WebWorksheet, WebCellArea) | Restablece los datos de origen |
| override [ToString](../../aspose.cells.gridweb.data/pivotcache/tostring/)() | Devuelve una cadena (String) que representa el Object actual |

### Observaciones

NOTA: Esta clase está ahora obsoleta. Por favor use GridPivotTable en su lugar. Esta clase será eliminada después de 6 meses desde agosto de 2014. Aspose se disculpa por cualquier inconveniente que haya experimentado.

Utiliza el método PivotCache para devolver un objeto PivotCache para un informe PivotTable (cada informe tiene solo una caché). Los datos de origen de PivotCache provienen de WebWorksheet, DataTable, etc.

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


