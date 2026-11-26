---
title: "Clase PivotCache"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Pivot.PivotCache. Representa la caché de memoria para algunos informes de PivotTable"
type: docs
url: /es/net/aspose.cells.pivot/pivotcache/
---
## PivotCache class

Representa la caché de memoria para algunos informes de PivotTable.

```csharp
public abstract class PivotCache : IDisposable
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [MissingItemsLimit](../../aspose.cells.pivot/pivotcache/missingitemslimit/) { get; set; } | Obtiene y establece el número de elementos no utilizados que se permiten antes de descartar los elementos no utilizados. Este valor DEBE ser mayor que -2 y menor que 1048577. [`PivotCacheMissingItemsLimitConst`](../pivotcachemissingitemslimitconst/); |
| abstract [SourceType](../../aspose.cells.pivot/pivotcache/sourcetype/) { get; } | Obtiene el [`PivotTableSourceType`](../pivottablesourcetype/). |

## Métodos

| Nombre | Descripción |
| --- | --- |
| abstract [Dispose](../../aspose.cells.pivot/pivotcache/dispose/)() | Liberar todos los recursos. |
| [GetPivotTables](../../aspose.cells.pivot/pivotcache/getpivottables/)() | Obtiene todas las tablas dinámicas con esta caché de tabla dinámica. |
| [Refresh](../../aspose.cells.pivot/pivotcache/refresh/#refresh)() | Actualiza los datos de la fuente de datos y calcula los datos para la vista de todas las tablas dinámicas cuya fuente de datos es esta caché de tabla dinámica. |
| [Refresh](../../aspose.cells.pivot/pivotcache/refresh/#refresh_1)(PivotTableRefreshOption) | Actualiza los datos de la fuente de datos y calcula los datos para la vista de todas las tablas dinámicas cuya fuente de datos es esta caché de tabla dinámica. |

### Observaciones

Todos los datos se recopilarán en esta caché, y la tabla dinámica solo obtendrá datos de esta caché, sin acceder directamente a la fuente de datos. Si la fuente de datos de algunas [`PivotTable`](../pivottable/) es la misma, usarán una caché de tabla dinámica.

### Ver también

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


