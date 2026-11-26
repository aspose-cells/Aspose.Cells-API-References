---
title: "TickLabels.RotationAngle"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad TickLabels. Representa el ángulo de rotación del texto en sentido horario"
type: docs
url: /es/net/aspose.cells.charts/ticklabels/rotationangle/
---
## TickLabels.RotationAngle property

Representa el ángulo de rotación del texto en sentido horario.

```csharp
public int RotationAngle { get; set; }
```

### Observaciones

0: No rotado.255: De arriba a abajo.-90: Hacia abajo.90: Hacia arriba.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TickLabelsPropertyRotationAngleDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            sheet.Cells["A1"].PutValue("Category 1");
            sheet.Cells["A2"].PutValue("Category 2");
            sheet.Cells["A3"].PutValue("Category 3");
            sheet.Cells["B1"].PutValue(100);
            sheet.Cells["B2"].PutValue(200);
            sheet.Cells["B3"].PutValue(300);

            // Añade un gráfico
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 20, 10);
            Chart chart = sheet.Charts[chartIndex];
            
            // Establecer origen de datos del Chart
            chart.NSeries.Add("B1:B3", true);
            chart.NSeries.CategoryData = "A1:A3";

            // Girar las etiquetas de marcas del eje de categorías 45 grados
            chart.CategoryAxis.TickLabels.RotationAngle = 45;

            // Guarda el libro de trabajo
            workbook.Save("TickLabelsRotationDemo.xlsx");
        }
    }
}
```

### Ver también

* class [TickLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


