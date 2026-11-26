---
title: "Axis.IsDisplayUnitLabelShown"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Axis. Representa si la etiqueta de unidad de visualización se muestra en el eje especificado"
type: docs
url: /es/net/aspose.cells.charts/axis/isdisplayunitlabelshown/
---
## Axis.IsDisplayUnitLabelShown property

Representa si la etiqueta de unidad de visualización se muestra en el eje especificado.

```csharp
public bool IsDisplayUnitLabelShown { get; set; }
```

### Observaciones

El valor predeterminado es True. Solo funciona cuando [`DisplayUnit`](../displayunit/) no es None.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyIsDisplayUnitLabelShownDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Datos de ejemplo
            worksheet.Cells["A1"].PutValue(500000);
            worksheet.Cells["A2"].PutValue(1000000);
            worksheet.Cells["A3"].PutValue(1500000);
            worksheet.Cells["B1"].PutValue(4);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(50);
            
            // Crear gráfico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:B3", true);
            
            // Configurar visibilidad de unidad de visualización y etiqueta
            chart.ValueAxis.DisplayUnit = DisplayUnitType.Millions;
            chart.ValueAxis.IsDisplayUnitLabelShown = true;
            
            workbook.Save("AxisPropertyIsDisplayUnitLabelShownDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


