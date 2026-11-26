---
title: "ChartFrame.Height"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ChartFrame. Obtiene o establece la altura del marco en unidades de 1/4000 del área del gráfico"
type: docs
url: /es/net/aspose.cells.charts/chartframe/height/
---
## ChartFrame.Height property

Obtiene o establece la altura del marco en unidades de 1/4000 del área del gráfico.

```csharp
[Obsolete("Use ChartFrame.HeightRatioToChart property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public virtual int Height { get; set; }
```

### Observaciones

¿Cómo convertir unidades de 1/4000 a píxeles? Altura en píxeles = Y * Chart.ChartObject.Height / 4000d;

NOTA: Este miembro está ahora obsoleto. Por favor, use la propiedad ChartFrame.HeightRatioToChart, en su lugar. Height = HeightRatioToChart * 4000. Esta propiedad será eliminada 12 meses después a partir de febrero de 2025. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartFramePropertyHeightDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
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
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Establecer origen de datos del Chart
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Acceder a las etiquetas de datos
            DataLabels dataLabels = chart.NSeries[0].DataLabels;
            
            // Establecer la propiedad Height
            dataLabels.Height = 200; // Set height to 200 pixels
            
            // Mostrar el valor de la altura
            Console.WriteLine("DataLabels Height: " + dataLabels.Height);
            
            // Guarda el libro de trabajo
            workbook.Save("ChartFramePropertyHeightDemo_out.xlsx");
        }
    }
}
```

### Ver también

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


