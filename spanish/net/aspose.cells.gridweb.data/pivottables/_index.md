---
title: "Clase PivotTables"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.GridWeb.Data.PivotTables class. Representa una colección de todos los objetos PivotTable."
type: docs
url: /es/net/aspose.cells.gridweb.data/pivottables/
---
## PivotTables class

Representa una colección de todos los objetos [`PivotTable`](../pivottable/)

```csharp
[Obsolete("This class is obsolete; use GridPivotTableCollection instead")]
public class PivotTables : ICollection
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Count](../../aspose.cells.gridweb.data/pivottables/count/) { get; } | Obtiene el número de elementos contenidos en la instancia de PivotTables |
| [IsSynchronized](../../aspose.cells.gridweb.data/pivottables/issynchronized/) { get; } | Obtiene un valor que indica si el acceso a PivotTables está sincronizado (seguro para subprocesos). |
| [Item](../../aspose.cells.gridweb.data/pivottables/item/) { get; } | Obtiene un objeto PivotTable por índice. (2 indexadores) |
| [Parent](../../aspose.cells.gridweb.data/pivottables/parent/) { get; } | Obtiene el objeto padre para el objeto especificado. Solo lectura. |
| [SyncRoot](../../aspose.cells.gridweb.data/pivottables/syncroot/) { get; } | Obtiene un objeto que puede usarse para sincronizar el acceso a PivotTables. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [Add](../../aspose.cells.gridweb.data/pivottables/add/#add)(PivotCache) | Agrega un objeto PivotTable del PivotCache especificado a una nueva hoja de cálculo |
| [Add](../../aspose.cells.gridweb.data/pivottables/add/#add_3)(PivotCache, string) | Agrega un objeto PivotTable del PivotCache especificado a una nueva hoja de cálculo |
| [Add](../../aspose.cells.gridweb.data/pivottables/add/#add_1)(PivotCache, WebWorksheet, WebCell) | Agrega un objeto PivotTable del PivotCache especificado a la hoja de cálculo especificada |
| [Add](../../aspose.cells.gridweb.data/pivottables/add/#add_2)(PivotCache, WebWorksheet, WebCell, string) | Agrega un objeto PivotTable del PivotCache especificado a la hoja de cálculo especificada |
| [Clear](../../aspose.cells.gridweb.data/pivottables/clear/)() | Elimina todos los objetos PivotTable y todos los objetos PivotCache en el control. |
| [Contains](../../aspose.cells.gridweb.data/pivottables/contains/)(string) | Devuelve true si existe una tabla pivote con el nombre tableName. |
| [CopyTo](../../aspose.cells.gridweb.data/pivottables/copyto/)(Array, int) | Copia toda la tabla dinámica a una matriz unidimensional compatible, comenzando en el índice especificado de la matriz de destino |
| [GetEnumerator](../../aspose.cells.gridweb.data/pivottables/getenumerator/)() | Devuelve un IEnumerator para las tablas dinámicas. |
| [Refresh](../../aspose.cells.gridweb.data/pivottables/refresh/)(PivotTable) | ReDataBinds la fuente de datos al informe de tabla dinámica. |
| [RefreshAll](../../aspose.cells.gridweb.data/pivottables/refreshall/)() | ReDataBinds la fuente de datos a todos los informes de tabla dinámica. |
| [Remove](../../aspose.cells.gridweb.data/pivottables/remove/)(PivotTable) | Elimina el objeto de tabla dinámica especificado de las tablas dinámicas y del PivotCache relacionado si no es utilizado por otra tabla dinámica. |
| [RemoveAt](../../aspose.cells.gridweb.data/pivottables/removeat/)(int) | Elimina el objeto de tabla dinámica especificado de las tablas dinámicas y del PivotCache relacionado si no es utilizado por otra tabla dinámica. |

### Observaciones

NOTA: Esta clase está ahora obsoleta. Por favor, use GridPivotTableCollection en su lugar. Esta clase será eliminada después de 6 meses desde agosto de 2014. Aspose se disculpa por cualquier inconveniente que haya experimentado.

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


