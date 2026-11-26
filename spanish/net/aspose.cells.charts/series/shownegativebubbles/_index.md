---
title: "Series.ShowNegativeBubbles"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad de Series. Verdadero si se muestran burbujas negativas para el grupo de gráficos. Válido solo para gráficos de burbujas"
type: docs
url: /es/net/aspose.cells.charts/series/shownegativebubbles/
---
## Series.ShowNegativeBubbles property

True si se muestran burbujas negativas para el grupo de gráfico. Válido solo para gráficos de burbujas.

```csharp
public bool ShowNegativeBubbles { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyShowNegativeBubblesDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo para el gráfico de burbujas
            worksheet.Cells["A1"].PutValue("X");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["A4"].PutValue(3);
            
            worksheet.Cells["B1"].PutValue("Y");
            worksheet.Cells["B2"].PutValue(2);
            worksheet.Cells["B3"].PutValue(-3);
            worksheet.Cells["B4"].PutValue(4);
            
            worksheet.Cells["C1"].PutValue("Size");
            worksheet.Cells["C2"].PutValue(5);
            worksheet.Cells["C3"].PutValue(6);
            worksheet.Cells["C4"].PutValue(7);

            // Agregar un gráfico de burbujas
            int chartIndex = worksheet.Charts.Add(ChartType.Bubble, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Establecer rango de datos del gráfico
            SeriesCollection seriesCollection = chart.NSeries;
            seriesCollection.Add("B2:B4", true);
            seriesCollection.CategoryData = "A2:A4";
            seriesCollection[0].BubbleSizes = "C2:C4";

            // Acceder a la primera serie y establecer la propiedad ShowNegativeBubbles
            Series series = chart.NSeries[0];
            series.ShowNegativeBubbles = true;

            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


