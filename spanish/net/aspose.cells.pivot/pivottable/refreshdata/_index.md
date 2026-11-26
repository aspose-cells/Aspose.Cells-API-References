---
title: "PivotTable.RefreshData"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método PivotTable. Actualiza los datos de su fuente de datos a la caché de pivote"
type: docs
url: /es/net/aspose.cells.pivot/pivottable/refreshdata/
---
## RefreshData() {#refreshdata}

Actualiza los datos de su fuente de datos a la caché de pivote.

```csharp
[Obsolete("Use PivotCache.Refresh() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public PivotRefreshState RefreshData()
```

### Observaciones

Recopilaremos datos de la fuente de datos a una caché de tabla dinámica, luego calcularemos los datos en la caché en las celdas. Y es mejor que simplemente llame a [`RefreshAll`](../../../aspose.cells/workbook/refreshall/) para actualizar y calcular todas las tablas dinámicas en el archivo, en lugar de actualizar una por una. NOTA: Este método está ahora obsoleto. En su lugar, utilice el método [`Refresh`](../../pivotcache/refresh/) y elimine el siguiente [`CalculateData`](../calculatedata/) porque esta tabla dinámica se calculará al actualizar la [`PivotCache`](../pivotcache/). Este método será eliminado 12 meses después, a partir de junio de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodRefreshDataDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de muestra para la tabla dinámica
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["A4"].PutValue("A");
            worksheet.Cells["B4"].PutValue(150);
            
            // Crear tabla dinámica
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Agregar campos de fila y de datos
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            
            // Actualizar y calcular los datos de la tabla dinámica
            pivotTable.CalculateData();
            pivotTable.RefreshData();
            
            // Guarda el libro de trabajo
            workbook.Save("PivotTableRefreshDataDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [PivotRefreshState](../../pivotrefreshstate/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## RefreshData(PivotTableRefreshOption) {#refreshdata_1}

Actualiza los datos y la configuración de la tabla dinámica desde su fuente de datos con opciones.

```csharp
[Obsolete("Use PivotCache.Refresh() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public PivotRefreshState RefreshData(PivotTableRefreshOption option)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| opción | PivotTableRefreshOption | Las opciones para actualizar la fuente de datos de la pivot table. |

### Observaciones

Recopilaremos datos de la fuente de datos a una caché de tabla dinámica, luego calcularemos los datos en la caché en las celdas. Y es mejor que simplemente llame a [`RefreshAll`](../../../aspose.cells/workbook/refreshall/) para actualizar y calcular todas las tablas dinámicas en el archivo, en lugar de actualizar una por una. NOTA: Este método está ahora obsoleto. En su lugar, utilice el método [`Refresh`](../../pivotcache/refresh/) y elimine el siguiente [`CalculateData`](../calculatedata/) porque esta tabla dinámica se calculará al actualizar la [`PivotCache`](../pivotcache/). Este método será eliminado 12 meses después, a partir de junio de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodRefreshDataWithPivotTableRefreshOptionDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo a partir del archivo Excel fuente
            Workbook workbook = new Workbook("example.xlsx");
            
            // Acceder a la hoja de cálculo que contiene la tabla dinámica
            Worksheet worksheet = workbook.Worksheets["PNL_AFS"];
            
            // Obtener la primera tabla dinámica en la hoja de cálculo
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // Configurar opciones de actualización
            PivotTableRefreshOption refreshOptions = new PivotTableRefreshOption();
            refreshOptions.ReserveMissingPivotItemType = ReserveMissingPivotItemType.None;
            
            // Actualizar los datos de la tabla dinámica con las opciones especificadas
            pivotTable.RefreshData(refreshOptions);
            pivotTable.CalculateData();
            
            // Guardar el libro de trabajo modificado
            workbook.Save("example_modified.xlsx");
        }
    }
}
```

### Ver también

* enum [PivotRefreshState](../../pivotrefreshstate/)
* class [PivotTableRefreshOption](../../pivottablerefreshoption/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


