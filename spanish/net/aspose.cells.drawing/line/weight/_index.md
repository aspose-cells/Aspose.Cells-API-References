---
title: "Line.Weight"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Line. Obtiene o establece el WeightType de la línea"
type: docs
url: /es/net/aspose.cells.drawing/line/weight/
---
## Line.Weight property

Obtiene o establece el [`WeightType`](../../weighttype/) de la línea.

```csharp
public WeightType Weight { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class LinePropertyWeightDemo
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
            
            // Establecer rango de datos del gráfico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Acceda al área del gráfico y establezca el grosor del borde
            ChartArea chartArea = chart.ChartArea;
            chartArea.Border.Weight = WeightType.MediumLine;

            // Guarda el libro de trabajo
            workbook.Save("LinePropertyWeightDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ver también

* enum [WeightType](../../weighttype/)
* class [Line](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


