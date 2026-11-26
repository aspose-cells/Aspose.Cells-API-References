---
title: "PivotOptions.DropZoneData"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PivotOptions. Especifica si un control para cada campo de PivotTable en el eje de datos de la tabla dinámica de origen aparece en el gráfico cuando dropZonesVisible está configurado como verdadero"
type: docs
url: /es/net/aspose.cells.charts/pivotoptions/dropzonedata/
---
## PivotOptions.DropZoneData property

Especifica si un control para cada campo de PivotTable en el eje de datos de la PivotTable de origen aparece en el gráfico cuando dropZonesVisible está configurado a true.

```csharp
public bool DropZoneData { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class PivotOptionsPropertyDropZoneDataDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Datos de muestra para la tabla dinámica
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("Books");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["A3"].PutValue("Electronics");
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["A4"].PutValue("Books");
            worksheet.Cells["B4"].PutValue(1500);

            // Crear tabla dinámica
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "D1", "SalesPivot");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Crear gráfico vinculado a la tabla dinámica
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 7, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.PivotSource = "SalesPivot";

            // Configurar opciones de tabla dinámica con DropZoneData habilitado
            PivotOptions pivotOptions = chart.PivotOptions;
            pivotOptions.DropZoneData = true;
            pivotOptions.DropZonesVisible = true;

            // Guardar el resultado
            workbook.Save("PivotOptionsDropZoneDataDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PivotOptions](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


