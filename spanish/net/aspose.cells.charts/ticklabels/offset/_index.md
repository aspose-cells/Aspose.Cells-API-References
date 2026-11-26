---
title: "TickLabels.Offset"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad TickLabels. Obtiene y establece la distancia de las etiquetas al eje de categoría. Esto se aplica solo al eje x de categoría"
type: docs
url: /es/net/aspose.cells.charts/ticklabels/offset/
---
## TickLabels.Offset property

Obtiene y establece la distancia de las etiquetas al eje de categoría. Esto se aplica solo al eje de categoría (x).

```csharp
public int Offset { get; set; }
```

### Observaciones

La distancia predeterminada es 100 por ciento, lo que representa el espaciado predeterminado entre las etiquetas del eje y la línea del eje. El valor puede ser un porcentaje entero de 0 a 1000, relativo al tamaño de fuente de la etiqueta del eje.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class TickLabelsPropertyOffsetDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["A4"].PutValue("C");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["B3"].PutValue(20);
            sheet.Cells["B4"].PutValue(30);

            // Añade un gráfico
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = sheet.Charts[chartIndex];
            
            // Establecer origen de datos del Chart
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Acceder al eje de valores
            Axis valueAxis = chart.ValueAxis;
            
            // Establecer el desplazamiento de TickLabels
            valueAxis.TickLabels.Offset = 50; // 50% offset from default position

            // Guarda el libro de trabajo
            workbook.Save("TickLabelsOffsetDemo.xlsx");
        }
    }
}
```

### Ver también

* class [TickLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


