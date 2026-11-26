---
title: "Series.BubbleScale"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Series. Obtiene o establece el factor de escala para las burbujas en el grupo de gráfico especificado. Puede ser un valor entero de 0 a 300 que corresponde a un porcentaje del tamaño predeterminado. Se aplica solo a gráficos de burbujas"
type: docs
url: /es/net/aspose.cells.charts/series/bubblescale/
---
## Series.BubbleScale property

Obtiene o establece el factor de escala para las burbujas en el grupo de gráfico especificado. Puede ser un valor entero de 0 (cero) a 300, correspondiente a un porcentaje del tamaño predeterminado. Se aplica solo a gráficos de burbujas.

```csharp
public int BubbleScale { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class SeriesPropertyBubbleScaleDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo para el gráfico de burbujas
            worksheet.Cells["A1"].PutValue("X");
            worksheet.Cells["B1"].PutValue("Y");
            worksheet.Cells["C1"].PutValue("Size");
            
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["C2"].PutValue(5);
            
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["C3"].PutValue(10);
            
            worksheet.Cells["A4"].PutValue(3);
            worksheet.Cells["B4"].PutValue(30);
            worksheet.Cells["C4"].PutValue(15);

            // Agregar un gráfico de burbujas
            int chartIndex = worksheet.Charts.Add(ChartType.Bubble, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Agregar series al gráfico
            int seriesIndex = chart.NSeries.Add("B2:B4", true);
            chart.NSeries[seriesIndex].XValues = "A2:A4";
            chart.NSeries[seriesIndex].BubbleSizes = "C2:C4";
            
            // Establecer la escala de burbujas para demostrar la propiedad
            chart.NSeries[seriesIndex].BubbleScale = 150; // Scale bubbles to 150% of default size
            
            // Personalizar la apariencia del gráfico
            chart.Title.Text = "Bubble Chart with Scaled Bubbles";
            chart.NSeries[seriesIndex].Area.FillFormat.SetOneColorGradient(Color.LightBlue, 0.5, Aspose.Cells.Drawing.GradientStyleType.Horizontal, 1);
            
            // Guarda el libro de trabajo
            workbook.Save("BubbleScaleDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


