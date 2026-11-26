---
title: "Chart.Style"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad del gráfico. Obtiene y establece el estilo incorporado"
type: docs
url: /es/net/aspose.cells.charts/chart/style/
---
## Chart.Style property

Obtiene y establece el estilo incorporado.

```csharp
public int Style { get; set; }
```

### Observaciones

Debe estar entre 1 y 48. Devuelve -1 si no está establecido.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyStyleDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo para el gráfico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B4"].PutValue(30);

            // Añade un gráfico
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart1 = worksheet.Charts[chartIndex];
            chart1.NSeries.Add("B2:B4", false);
            chart1.NSeries.CategoryData = "A2:A4";

            // Crea otro gráfico y copia el estilo del primer gráfico
            chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 10, 20, 18);
            Aspose.Cells.Charts.Chart chart2 = worksheet.Charts[chartIndex];
            chart2.NSeries.Add("B2:B4", false);
            chart2.NSeries.CategoryData = "A2:A4";
            
            // Demostrar el uso de la propiedad Style
            chart2.Style = chart1.Style;

            // Guarda el libro de trabajo
            workbook.Save("ChartStyleDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


