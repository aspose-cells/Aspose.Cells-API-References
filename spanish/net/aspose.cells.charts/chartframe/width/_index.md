---
title: "ChartFrame.Width"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ChartFrame. Obtiene o establece el ancho del marco en unidades de 1/4000 del área del gráfico"
type: docs
url: /es/net/aspose.cells.charts/chartframe/width/
---
## ChartFrame.Width property

Obtiene o establece el ancho del marco en unidades de 1/4000 del área del gráfico.

```csharp
[Obsolete("Use ChartFrame.WidthRatioToChart property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public virtual int Width { get; set; }
```

### Observaciones

¿Cómo convertir unidades de 1/4000 a píxeles? Ancho en píxeles = Ancho * Chart.ChartObject.Height / 4000d;

NOTA: Este miembro está ahora obsoleto. Por favor use la propiedad ChartFrame.WidthRatioToChart, en su lugar. Ancho = WidthRatioToChart * 4000; Esta propiedad será eliminada 12 meses después a partir de febrero de 2025. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartFramePropertyWidthDemo
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

            // Agregar un gráfico y obtener su marco del gráfico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            ChartFrame chartFrame = chart.ChartArea;

            // Establecer y mostrar el ancho original
            chartFrame.Width = 800;
            Console.WriteLine("Original Width: " + chartFrame.Width);

            // Modificar el ancho
            chartFrame.Width = 1000;
            Console.WriteLine("Modified Width: " + chartFrame.Width);

            // Guarda el libro de trabajo
            workbook.Save("ChartFrameWidthDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


