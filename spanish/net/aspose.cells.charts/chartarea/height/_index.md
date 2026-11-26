---
title: "ChartArea.Height"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ChartArea. Obtiene o establece el desplazamiento vertical desde la fila de su esquina inferior derecha en unidades de 1/4000 del área del gráfico"
type: docs
url: /es/net/aspose.cells.charts/chartarea/height/
---
## ChartArea.Height property

Obtiene o establece el desplazamiento vertical desde la fila de su esquina inferior‑derecha, en unidades de 1/4000 del área del gráfico.

```csharp
[Obsolete("Use ChartArea.HeightRatioToChart property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public override int Height { get; set; }
```

### Observaciones

NOTA: Este miembro está ahora obsoleto. Por favor, use la propiedad ChartArea.HeightRatioToChart, en su lugar. Height = HeightRatioToChart * 4000. Esta propiedad será eliminada 12 meses después, a partir de febrero de 2025. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartAreaPropertyHeightDemo
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
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Establecer origen de datos del Chart
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Acceder al área del gráfico
            ChartArea chartArea = chart.ChartArea;

            // Demostrar la propiedad Height
            Console.WriteLine("Original Chart Area Height: " + chartArea.Height);
            
            // Modificar la altura
            chartArea.Height = 500;
            Console.WriteLine("Modified Chart Area Height: " + chartArea.Height);

            // Guarda el libro de trabajo
            workbook.Save("ChartAreaHeightDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ChartArea](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


