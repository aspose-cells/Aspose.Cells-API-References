---
title: "Clase PivotField"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.GridWeb.Data.PivotField. Representa un campo en un informe de tabla dinámica. El objeto PivotField es un miembro de la colección PivotFields.  NOTA Esta clase está ahora obsoleta. En su lugar, por favor use GridPivotField. Esta clase será eliminada después de 6 meses desde agosto de 2014. Aspose se disculpa por cualquier inconveniente que haya experimentado"
type: docs
url: /es/net/aspose.cells.gridweb.data/pivotfield/
---
## PivotField class

Representa un campo en un informe de tabla dinámica. El objeto PivotField es un miembro de la colección [`PivotFields`](../pivotfields/).  NOTA: Esta clase está ahora obsoleta. En su lugar, por favor use GridPivotField. Esta clase será eliminada después de 6 meses desde agosto de 2014. Aspose se disculpa por cualquier inconveniente que haya experimentado.

```csharp
[Obsolete("This class is obsolete; use GridPivotField instead")]
public class PivotField
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Caption](../../aspose.cells.gridweb.data/pivotfield/caption/) { get; set; } | El texto de la etiqueta para el campo dinámico se muestra en el informe. Por defecto muestra el nombre. |
| [FieldItems](../../aspose.cells.gridweb.data/pivotfield/fielditems/) { get; } | Obtiene los datos del campo especificado. |
| [Function](../../aspose.cells.gridweb.data/pivotfield/function/) { get; set; } | Representa la función utilizada para resumir el campo de la tabla dinámica (solo campos de datos). La función predeterminada es Count. |
| [Name](../../aspose.cells.gridweb.data/pivotfield/name/) { get; } | Obtiene el nombre. |
| [Orientation](../../aspose.cells.gridweb.data/pivotfield/orientation/) { get; set; } | Representa la ubicación del campo en el informe PivotTable especificado. |
| [Position](../../aspose.cells.gridweb.data/pivotfield/position/) { get; set; } | Representa la posición del campo (primero, segundo, tercero, etc.) entre todos los campos en su orientación (Rows, Columns, Pages). Debe llamar al método get después de invocar Pivottable.DataBind. |
| [SortOrder](../../aspose.cells.gridweb.data/pivotfield/sortorder/) { get; set; } | Representa el orden usado para ordenar el campo PivotTable especificado. |

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


