---
title: "Clase AxisBins"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Charts.AxisBins. Representa contenedores de eje"
type: docs
url: /es/net/aspose.cells.charts/axisbins/
---
## AxisBins class

Representa los contenedores del eje.

```csharp
public class AxisBins
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Count](../../aspose.cells.charts/axisbins/count/) { get; set; } | Obtiene o establece la cantidad de contenedores de eje |
| [IsAutomatic](../../aspose.cells.charts/axisbins/isautomatic/) { get; set; } | Indica si los contenedores de eje son automáticos. |
| [IsByCategory](../../aspose.cells.charts/axisbins/isbycategory/) { get; set; } | Indica si la agrupación de datos por categoría está habilitada. |
| [Overflow](../../aspose.cells.charts/axisbins/overflow/) { get; set; } | Obtiene o establece el desbordamiento de los contenedores de eje |
| [Underflow](../../aspose.cells.charts/axisbins/underflow/) { get; set; } | Obtiene o establece el subdesbordamiento de los contenedores de eje |
| [Width](../../aspose.cells.charts/axisbins/width/) { get; set; } | Obtiene o establece el ancho del contenedor de eje. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [ResetOverflow](../../aspose.cells.charts/axisbins/resetoverflow/)() | (**Obsolete.**) Restablecer el desbordamiento |
| [ResetUnderflow](../../aspose.cells.charts/axisbins/resetunderflow/)() | (**Obsolete.**) Restablecer el subdesbordamiento |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class AxisBinsDemo
    {
        public static void AxisBinsExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            // Agregar una nueva hoja de trabajo
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar algunos datos de ejemplo
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["A4"].PutValue(40);
            worksheet.Cells["A5"].PutValue(50);

            // Agregar un gráfico a la hoja de cálculo
            int chartIndex = worksheet.Charts.Add(ChartType.Histogram, 5, 0, 25, 10);
            Chart chart = worksheet.Charts[chartIndex];

            // Agregar series de datos al gráfico
            chart.NSeries.Add("A1:A5", true);

            // Acceder al eje de valores
            Axis valueAxis = chart.ValueAxis;

            // Acceder a los contenedores del eje de valores
            AxisBins bins = valueAxis.Bins;

            // Establecer propiedades para los contenedores
            bins.IsByCategory = false;
            bins.IsAutomatic = true;
            bins.Width = 10.0;
            bins.Count = 5;
            bins.Overflow = 60.0;
            bins.Underflow = 0.0;

            // Restablecer desbordamiento y subdesbordamiento
            //bins.ResetOverflow();
            //bins.ResetUnderflow();

            // Guarda el libro de trabajo
            workbook.Save("AxisBinsExample.xlsx");
            workbook.Save("AxisBinsExample.pdf");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


