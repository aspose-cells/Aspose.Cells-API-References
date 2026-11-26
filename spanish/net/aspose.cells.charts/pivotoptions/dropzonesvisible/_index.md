---
title: "PivotOptions.DropZonesVisible"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PivotOptions. Especifica si algún control de tabla dinámica puede aparecer en el gráfico de tabla dinámica"
type: docs
url: /es/net/aspose.cells.charts/pivotoptions/dropzonesvisible/
---
## PivotOptions.DropZonesVisible property

Especifica si algún control pivot puede aparecer en el gráfico pivot.

```csharp
public bool DropZonesVisible { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotOptionsPropertyDropZonesVisibleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Datos de muestra para la tabla dinámica
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

            // Configurar opciones de tabla dinámica con DropZonesVisible
            PivotOptions pivotOptions = chart.PivotOptions;
            pivotOptions.DropZonesVisible = true;

            workbook.Save("PivotOptionsDropZonesVisibleDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PivotOptions](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


