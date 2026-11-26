---
title: "Floor.Border"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Floor. Obtiene o establece la línea del borde"
type: docs
url: /es/net/aspose.cells.charts/floor/border/
---
## Floor.Border property

Obtiene o establece el borde [`Line`](../../../aspose.cells.drawing/line/).

```csharp
public Line Border { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class FloorPropertyBorderDemo
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

            // Agregar un gráfico de columnas 3D
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Obtener el Floor del gráfico
            Floor floor = chart.Floor;

            // Establecer propiedades del borde modificando el borde existente en lugar de crear uno nuevo
            floor.Border.Color = Color.Red;
            floor.Border.Weight = WeightType.MediumLine;
            floor.Border.DashType = MsoLineDashStyle.DashDot;
            floor.Border.IsVisible = true;
            floor.Border.Transparency = 0.5;

            // Guarda el libro de trabajo
            workbook.Save("FloorBorderDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Line](../../../aspose.cells.drawing/line/)
* class [Floor](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


