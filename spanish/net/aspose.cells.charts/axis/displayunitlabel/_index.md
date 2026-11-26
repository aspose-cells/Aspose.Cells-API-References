---
title: "Axis.DisplayUnitLabel"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Axis. Representa una etiqueta de unidad en un eje del gráfico especificado. Las etiquetas de unidad son útiles para graficar valores grandes, por ejemplo en millones o miles de millones"
type: docs
url: /es/net/aspose.cells.charts/axis/displayunitlabel/
---
## Axis.DisplayUnitLabel property

Representa una etiqueta de unidad en un eje del gráfico especificado. Las etiquetas de unidad son útiles para graficar valores grandes, por ejemplo, en millones o miles de millones.

```csharp
public DisplayUnitLabel DisplayUnitLabel { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyDisplayUnitLabelDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue(1000);
            worksheet.Cells["A2"].PutValue(2000);
            worksheet.Cells["A3"].PutValue(3000);
            worksheet.Cells["A4"].PutValue(4000);
            
            // Crear gráfico
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Establecer rango de datos del gráfico
            chart.NSeries.Add("A1:A4", true);
            
            // Configurar unidad de visualización y etiqueta
            chart.ValueAxis.DisplayUnit = Aspose.Cells.Charts.DisplayUnitType.Thousands;
            chart.ValueAxis.IsDisplayUnitLabelShown = true;
            
            // Salida del texto de la etiqueta de unidad de visualización
            Console.WriteLine("Display Unit Label: " + chart.ValueAxis.DisplayUnitLabel.Text);
            
            // Guarda el libro de trabajo
            workbook.Save("AxisPropertyDisplayUnitLabelDemo_out.xlsx");
        }
    }
}
```

### Ver también

* class [DisplayUnitLabel](../../displayunitlabel/)
* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


