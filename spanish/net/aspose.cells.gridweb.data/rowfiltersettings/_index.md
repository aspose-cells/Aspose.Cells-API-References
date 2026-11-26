---
title: "Clase RowFilterSettings"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.GridWeb.Data.RowFilterSettings class. Descripción resumida para RowFilter"
type: docs
url: /es/net/aspose.cells.gridweb.data/rowfiltersettings/
---
## RowFilterSettings class

Descripción resumida para RowFilter.

```csharp
[Obsolete("This class is obsolete; use  GridWorksheet.AddAutoFilter/FilterString for autofilter /custom filter settings")]
public class RowFilterSettings : IComparer, ISerializable
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Criteria](../../aspose.cells.gridweb.data/rowfiltersettings/criteria/) { get; set; } | La cadena de criterios de filtro. |
| [EnableAutoFilter](../../aspose.cells.gridweb.data/rowfiltersettings/enableautofilter/) { get; set; } | Habilita el filtrado automático. La HeaderRow mostrará botones desplegables para permitir al usuario seleccionar el valor de la columna a filtrar. |
| [EndColumn](../../aspose.cells.gridweb.data/rowfiltersettings/endcolumn/) { get; set; } | El número de fila final del rango de filtro. Si este valor se establece en -1, se utiliza el número de la última fila de la hoja. |
| [HeaderRow](../../aspose.cells.gridweb.data/rowfiltersettings/headerrow/) { get; set; } | El número de fila de encabezado que mostrará los botones desplegables de filtro. |
| [StartColumn](../../aspose.cells.gridweb.data/rowfiltersettings/startcolumn/) { get; set; } | El número de fila inicial del rango de filtro. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [BuildAutoFilterCriteria](../../aspose.cells.gridweb.data/rowfiltersettings/buildautofiltercriteria/)() | Construye la cadena de criterios a partir de la configuración de filtro automático. |
| [ClearFilter](../../aspose.cells.gridweb.data/rowfiltersettings/clearfilter/)() | Borra todas las configuraciones de filtro y muestra todas las filas. |
| [CustomFilter](../../aspose.cells.gridweb.data/rowfiltersettings/customfilter/)(int, ICustomFilter) | Especifica un filtro personalizado. |
| [FilterRows](../../aspose.cells.gridweb.data/rowfiltersettings/filterrows/)() | Filtra filas usando la cadena de criterios. |

### Observaciones

NOTA: Esta clase está ahora obsoleta. Esta clase será eliminada después de 6 meses desde agosto de 2014. puede usar GridWorksheet AddAutoFilter/FilterString para configuraciones de autofiltro / filtro personalizado. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ver también

* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


