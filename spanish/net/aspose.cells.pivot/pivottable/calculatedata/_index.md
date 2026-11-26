---
title: "PivotTable.CalculateData"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método PivotTable. Calcula los datos de la tabla dinámica en las celdas"
type: docs
url: /es/net/aspose.cells.pivot/pivottable/calculatedata/
---
## CalculateData() {#calculatedata_1}

Calcula los datos de la tabla dinámica en celdas.

```csharp
public void CalculateData()
```

### Observaciones

Este método solo calcula los datos con la información almacenada en caché en el [`PivotCache`](../pivotcache/). Por lo tanto, si deseas calcular con la fuente de datos más reciente, por favor usa el método [`Refresh`](../../pivotcache/refresh/) para calcular. Si solo se cambió la configuración de la tabla dinámica, `CalculateData` es suficiente.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodCalculateDataDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Date");
            worksheet.Cells["B1"].PutValue("Sales");
            
            DateTime baseDate = new DateTime(2021, 11, 1);
            for (int i = 0; i < 15; i++)
            {
                worksheet.Cells[$"A{i+2}"].PutValue(baseDate.AddDays(i));
                worksheet.Cells[$"B{i+2}"].PutValue(100 + i * 10);
            }

            // Crear tabla dinámica - corregido asegurando parámetros correctos
            int pivotIndex = worksheet.PivotTables.Add("A1:B16", "D3", "PivotTable");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Agregar campos a la tabla dinámica
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Date");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Aplicar filtro de fecha
            PivotField dateField = pivotTable.RowFields[0];
            dateField.FilterByDate(PivotFilterType.November, new DateTime(2021, 1, 1), new DateTime(2021, 12, 31));
            
            // Calcular datos de la tabla dinámica
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Guarda el libro de trabajo
            workbook.Save("PivotTableCalculateDataDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## CalculateData(PivotTableCalculateOption) {#calculatedata}

Calcula la tabla dinámica con opciones.

```csharp
public PivotTable[] CalculateData(PivotTableCalculateOption option)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| opción | PivotTableCalculateOption | Las opciones para calcular la tabla dinámica |

### Valor de retorno

Devuelve todas las tablas dinámicas que han sido calculadas. Si [`RefreshData`](../../pivottablecalculateoption/refreshdata/) es verdadero, todas las tablas dinámicas basadas en la misma caché de pivote se calcularán juntas.

### Observaciones

Si [`RefreshData`](../../pivottablecalculateoption/refreshdata/) es verdadero, este método actualizará la caché de pivote desde la fuente de datos, y luego calculará todas las tablas dinámicas basadas en la misma caché de pivote. De lo contrario, solo se calculará con los datos almacenados en caché en la caché de pivote.

### Ejemplos

```csharp
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodCalculateDataWithPivotTableCalculateOptionDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Datos de ejemplo
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Crear tabla dinámica
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Configurar tabla dinámica
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Value");

            // Establecer opciones de cálculo
            PivotTableCalculateOption options = new PivotTableCalculateOption
            {
                RefreshData = true,
                ReserveMissingPivotItemType = ReserveMissingPivotItemType.All
            };

            // Calcular con opciones
            pivotTable.CalculateData(options);

            workbook.Save("PivotTableCalculateDataDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PivotTableCalculateOption](../../pivottablecalculateoption/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


