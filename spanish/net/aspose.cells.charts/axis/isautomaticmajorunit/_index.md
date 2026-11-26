---
title: "Axis.IsAutomaticMajorUnit"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Axis. Indica si la unidad principal del eje se asigna automáticamente"
type: docs
url: /es/net/aspose.cells.charts/axis/isautomaticmajorunit/
---
## Axis.IsAutomaticMajorUnit property

Indica si la unidad principal del eje se asigna automáticamente.

```csharp
public bool IsAutomaticMajorUnit { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyIsAutomaticMajorUnitDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo para el gráfico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            
            // Añade un gráfico
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Establecer origen de datos del Chart
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // Verificar y mostrar el estado automático de la unidad principal
            Console.WriteLine("IsAutomaticMajorUnit (default): " + chart.ValueAxis.IsAutomaticMajorUnit);
            
            // Desactivar la unidad mayor automática y establecer un valor personalizado
            chart.ValueAxis.IsAutomaticMajorUnit = false;
            chart.ValueAxis.MajorUnit = 5;
            Console.WriteLine("IsAutomaticMajorUnit (after change): " + chart.ValueAxis.IsAutomaticMajorUnit);
        }
    }
}
```

### Ver también

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


