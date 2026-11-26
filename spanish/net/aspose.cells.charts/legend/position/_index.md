---
title: "Legend.Position"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Legend. Obtiene o establece el tipo de posición de la leyenda"
type: docs
url: /es/net/aspose.cells.charts/legend/position/
---
## Legend.Position property

Obtiene o establece el tipo de posición de la leyenda.

```csharp
public LegendPositionType Position { get; set; }
```

### Observaciones

La posición predeterminada es a la derecha. Si la leyenda está en el lado izquierdo o derecho del gráfico, establecer la propiedad Legend.X no tendrá efecto. Si la leyenda está en la parte superior o inferior del gráfico, establecer la propiedad Legend.Y no tendrá efecto.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class LegendPropertyPositionDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo para el gráfico
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
            chart.SetChartDataRange("A1:B4", true);

            // Establecer la posición de la leyenda
            chart.Legend.Position = LegendPositionType.Left;

            // Guarda el libro de trabajo
            workbook.Save("LegendPositionDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [LegendPositionType](../../legendpositiontype/)
* class [Legend](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


