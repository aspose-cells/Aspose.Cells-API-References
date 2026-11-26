---
title: "Clase PivotFieldGroupOptions"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Pivot.PivotFieldGroupOptions. Opciones para la configuración de agrupación de campos dinámicos"
type: docs
url: /es/net/aspose.cells.pivot/pivotfieldgroupoptions/
---
## PivotFieldGroupOptions class

Opciones para la configuración de agrupación del campo de tabla dinámica.

```csharp
public class PivotFieldGroupOptions
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [PivotFieldGroupOptions](pivotfieldgroupoptions/)() | El constructor predeterminado. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [DiscreteGroupItems](../../aspose.cells.pivot/pivotfieldgroupoptions/discretegroupitems/) { get; set; } | Obtiene y establece los elementos de grupo discretos. |
| [EndDate](../../aspose.cells.pivot/pivotfieldgroupoptions/enddate/) { get; set; } | Obtiene o establece el valor final del rango de agrupación. |
| [EndNumber](../../aspose.cells.pivot/pivotfieldgroupoptions/endnumber/) { get; set; } | Obtiene o establece el valor final del rango de agrupación. |
| [GroupType](../../aspose.cells.pivot/pivotfieldgroupoptions/grouptype/) { get; set; } | Obtiene o establece el tipo de agrupación para el campo dinámico. Solo para campos dinámicos de fecha y hora. |
| [GroupTypes](../../aspose.cells.pivot/pivotfieldgroupoptions/grouptypes/) { get; set; } | Obtiene o establece el tipo de agrupación para el campo dinámico. |
| [Interval](../../aspose.cells.pivot/pivotfieldgroupoptions/interval/) { get; set; } | Obtiene o establece el tamaño del intervalo para cada grupo. |
| [IsAutoEnd](../../aspose.cells.pivot/pivotfieldgroupoptions/isautoend/) { get; set; } | Obtiene o establece un valor que indica si el valor final se determina automáticamente. |
| [IsAutoStart](../../aspose.cells.pivot/pivotfieldgroupoptions/isautostart/) { get; set; } | Obtiene o establece un valor que indica si el valor inicial se determina automáticamente. |
| [NewPivotField](../../aspose.cells.pivot/pivotfieldgroupoptions/newpivotfield/) { get; set; } | Obtiene o establece un valor que indica si se deben crear nuevos campos dinámicos después de la agrupación. |
| [StartDate](../../aspose.cells.pivot/pivotfieldgroupoptions/startdate/) { get; set; } | Obtiene o establece el valor inicial del rango de agrupación. |
| [StartNumber](../../aspose.cells.pivot/pivotfieldgroupoptions/startnumber/) { get; set; } | Obtiene o establece el valor inicial del rango de agrupación. |

### Ejemplos

```csharp

[C#]

// Cargar el libro de trabajo de ejemplo
Workbook wb = new Workbook("sampleGroupPivotFieldsInPivotTable.xlsx");
// Acceder a la segunda hoja de cálculo y su tabla dinámica
PivotTable pt = wb.Worksheets[1].PivotTables[0];
// Agrupar el primer campo de fila (un campo de fecha) por meses y trimestres
PivotFieldGroupOptions options = new PivotFieldGroupOptions();
options.StartDate = new DateTime(2008, 1, 1);
options.EndDate = new DateTime(2008, 9, 5);
options.GroupTypes = new PivotGroupByType[] { PivotGroupByType.Months, PivotGroupByType.Quarters };
pt.RowFields[0].Group(options);
// Calcular los datos de la tabla dinámica y guardar el archivo de salida
pt.CalculateData();
wb.Save("outputGroupPivotFieldsInPivotTable.xlsx");

[Visual Basic]

'Load the sample workbook
Dim wb As New Workbook("sampleGroupPivotFieldsInPivotTable.xlsx")
'Access the second worksheet and its pivot table
Dim pt As PivotTable = wb.Worksheets(1).PivotTables(0)
'Group the first row field (a date field) by months and quarters
Dim options As New PivotFieldGroupOptions()
options.StartDate = New DateTime(2008, 1, 1)
options.EndDate = New DateTime(2008, 9, 5)
options.GroupTypes = New PivotGroupByType() {PivotGroupByType.Months, PivotGroupByType.Quarters}
pt.RowFields(0).Group(options)
'Calculate the pivot table data and save the output file
pt.CalculateData()
wb.Save("outputGroupPivotFieldsInPivotTable.xlsx")
```

### Ver también

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


