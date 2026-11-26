---
title: "ChartFrame.Y"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ChartFrame. Obtiene o establece la coordenada y de la esquina superior izquierda en unidades de 1/4000 del área del gráfico"
type: docs
url: /es/net/aspose.cells.charts/chartframe/y/
---
## ChartFrame.Y property

Obtiene o establece la coordenada y de la esquina superior izquierda en unidades de 1/4000 del área del gráfico.

```csharp
[Obsolete("Use ChartFrame.YRatioToChart property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public virtual int Y { get; set; }
```

### Observaciones

Cómo convertir unidades de 1/4000 a píxeles? Y en píxeles = Y * Chart.ChartObject.Height / 4000d;

NOTA: Este miembro está ahora obsoleto. Por favor use la propiedad ChartFrame.YRatioToChart, en su lugar. Y = YRatioToChart * 4000. Esta propiedad será eliminada 12 meses después a partir de febrero de 2025. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartFramePropertyYDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            Cells cells = sheet.Cells;
            cells["A1"].PutValue("Category");
            cells["A2"].PutValue("A");
            cells["A3"].PutValue("B");
            cells["A4"].PutValue("C");
            cells["B1"].PutValue("Value");
            cells["B2"].PutValue(10);
            cells["B3"].PutValue(20);
            cells["B4"].PutValue(30);

            // Agregar gráfico
            int chartIndex = sheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = sheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B4", true);

            // Acceder al título del gráfico y establecer la posición Y
            chart.Title.Text = "Sample Chart";
            chart.Title.Y = 1000; // Demonstrate Y property usage

            // Guarda el libro de trabajo
            workbook.Save("ChartFramePropertyYDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


