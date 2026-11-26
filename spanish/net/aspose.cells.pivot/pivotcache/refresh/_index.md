---
title: "PivotCache.Refresh"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método PivotCache. Actualiza los datos desde la fuente de datos y calcula los datos para la vista de todas las pivottables cuya fuente de datos es este pivot cache."
type: docs
url: /es/net/aspose.cells.pivot/pivotcache/refresh/
---
## Refresh(PivotTableRefreshOption) {#refresh_1}

Actualiza los datos de la fuente de datos y calcula los datos para la vista de todas las tablas dinámicas cuya fuente de datos es esta caché de tabla dinámica.

```csharp
public PivotRefreshState Refresh(PivotTableRefreshOption option)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| opción | PivotTableRefreshOption | Las opciones para actualizar la fuente de datos de la pivot table. |

### Observaciones

Es mejor que puedas simplemente llamar a [`RefreshAll`](../../../aspose.cells/workbook/refreshall/) para actualizar todas las pivot tables y gráficos en el archivo.

### Ver también

* enum [PivotRefreshState](../../pivotrefreshstate/)
* class [PivotTableRefreshOption](../../pivottablerefreshoption/)
* class [PivotCache](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Refresh() {#refresh}

Actualiza los datos de la fuente de datos y calcula los datos para la vista de todas las tablas dinámicas cuya fuente de datos es esta caché de tabla dinámica.

```csharp
public PivotRefreshState Refresh()
```

### Observaciones

Si tanto table1 como table2 usan esta caché, las dos tablas se calcularán. Es mejor que puedas simplemente llamar a [`RefreshAll`](../../../aspose.cells/workbook/refreshall/) para actualizar todas las pivot tables y gráficos en el archivo.

### Ver también

* enum [PivotRefreshState](../../pivotrefreshstate/)
* class [PivotCache](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


