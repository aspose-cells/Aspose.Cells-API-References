---
title: "PivotOptions.DropZoneFilter"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PivotOptions. Especifica si un control para cada campo de PivotTable en el eje de página de PivotTable de la tabla dinámica de origen aparece en el gráfico cuando dropZonesVisible está configurado como verdadero"
type: docs
url: /es/net/aspose.cells.charts/pivotoptions/dropzonefilter/
---
## PivotOptions.DropZoneFilter property

Especifica si un control para cada campo de PivotTable en el eje de página de la PivotTable de origen aparece en el gráfico cuando dropZonesVisible está configurado a true.

```csharp
public bool DropZoneFilter { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class PivotOptionsPropertyDropZoneFilterDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Datos de ejemplo
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("A");
            worksheet.Cells["B4"].PutValue(30);
            worksheet.Cells["A5"].PutValue("B");
            worksheet.Cells["B5"].PutValue(40);

            // Crear tabla dinámica
            int pivotIndex = worksheet.PivotTables.Add("=A1:B5", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Crear gráfico vinculado a la tabla dinámica
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 7, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.PivotSource = "PivotTable1";

            // Configurar opciones de tabla dinámica con DropZoneFilter
            PivotOptions pivotOptions = chart.PivotOptions;
            pivotOptions.DropZoneFilter = true;
            pivotOptions.DropZonesVisible = true;

            workbook.Save("PivotOptionsDropZoneFilterDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PivotOptions](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


