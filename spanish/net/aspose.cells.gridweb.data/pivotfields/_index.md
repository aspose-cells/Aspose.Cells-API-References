---
title: "Clase PivotFields"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.GridWeb.Data.PivotFields. Representa una colección de todos los objetos PivotField en un informe de tabla dinámica"
type: docs
url: /es/net/aspose.cells.gridweb.data/pivotfields/
---
## PivotFields class

Representa una colección de todos los objetos [`PivotField`](../pivotfield/) en un informe de PivotTable.

```csharp
[Obsolete("This class is obsolete; use GridPivotFieldCollection instead")]
public class PivotFields : ICollection
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Count](../../aspose.cells.gridweb.data/pivotfields/count/) { get; } | Obtiene el número de elementos contenidos en la instancia de PivotFields |
| [IsSynchronized](../../aspose.cells.gridweb.data/pivotfields/issynchronized/) { get; } | Obtiene un valor que indica si el acceso a PivotFields está sincronizado (seguro para subprocesos). |
| [Item](../../aspose.cells.gridweb.data/pivotfields/item/) { get; } | Obtiene un PivotField por índice. (2 indexadores) |
| [Parent](../../aspose.cells.gridweb.data/pivotfields/parent/) { get; } | Obtiene el objeto padre para el objeto especificado. Solo lectura. |
| [SyncRoot](../../aspose.cells.gridweb.data/pivotfields/syncroot/) { get; } | Obtiene un objeto que puede usarse para sincronizar el acceso a PivotFields. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [CopyTo](../../aspose.cells.gridweb.data/pivotfields/copyto/)(Array, int) | Copia todo el PivotField a una Matriz unidimensional compatible, comenzando en el índice especificado de la matriz de destino |
| [GetEnumerator](../../aspose.cells.gridweb.data/pivotfields/getenumerator/)() | Devuelve un IEnumerator para los PivotFields. |
| [IndexOf](../../aspose.cells.gridweb.data/pivotfields/indexof/)(PivotField) | Obtiene el índice del PivotField especificado. |

### Observaciones

NOTA: Esta clase está ahora obsoleta. Por favor use GridPivotFieldCollection en su lugar. Esta clase será eliminada después de 6 meses desde agosto de 2014. Aspose se disculpa por cualquier inconveniente que pueda haber experimentado.

### Ejemplos

```csharp

 [C#]

 //Obtiene los PivotFields de PivotTable[0]
 PivotField field1 = GridWeb1.WebWorksheets.PivotTables[0].PivotFields["field1"];
 PivotField field2 = GridWeb1.WebWorksheets.PivotTables[0].PivotFields["field2"];
 PivotField field3 = GridWeb1.WebWorksheets.PivotTables[0].PivotFields["field3"];
 PivotField field4 = GridWeb1.WebWorksheets.PivotTables[0].PivotFields["field4"];

 //Establece la ubicación de los PivotFields
 field1.Orientation = PivotFieldOrientation.RowField;
 field2.Orientation = PivotFieldOrientation.RowField;
 field3.Orientation = PivotFieldOrientation.ColumnField;
 field4.Orientation = PivotFieldOrientation.DataField;

 //Establece la función del campo de datos
 field3.Function = PivotFieldFunction.Sum;

 //Cambia el orden de los campos de fila
 field2.Position = 1; //Or field1.Position = 2;

 [VB]

 'Gets PivotFields of PivotTable[0]
 Dim field1 As PivotField =  GridWeb1.WebWorksheets.PivotTables(0).PivotFields("field1")
 Dim field2 As PivotField =  GridWeb1.WebWorksheets.PivotTables(0).PivotFields("field2")
 Dim field3 As PivotField =  GridWeb1.WebWorksheets.PivotTables(0).PivotFields("field3")
 Dim field4 As PivotField =  GridWeb1.WebWorksheets.PivotTables(0).PivotFields("field4")

 'Sets Location of PivotFields
 field1.Orientation = PivotFieldOrientation.RowField
 field2.Orientation = PivotFieldOrientation.RowField
 field3.Orientation = PivotFieldOrientation.ColumnField
 field4.Orientation = PivotFieldOrientation.DataField

 'Sets function of data field
 field3.Function = PivotFieldFunction.Sum
 'Changes row fields order
 field2.Position = 1 'Or field1.Position = 2;

```

### Ver también

* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


