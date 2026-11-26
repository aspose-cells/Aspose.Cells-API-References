---
title: "Series.Has3DEffect"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad de Series. Verdadero si la serie tiene una apariencia tridimensional"
type: docs
url: /es/net/aspose.cells.charts/series/has3deffect/
---
## Series.Has3DEffect property

True si la serie tiene una apariencia tridimensional.

```csharp
public bool Has3DEffect { get; set; }
```

### Observaciones

Se aplica solo a gráficos Bubble o Bubble3D.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyHas3DEffectDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);
            worksheet.Cells["C1"].PutValue("Q1");
            worksheet.Cells["C2"].PutValue("Q2");
            worksheet.Cells["C3"].PutValue("Q3");

            // Añade un gráfico
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Agregar serie
            int seriesIndex = chart.NSeries.Add("A1:B3", true);
            chart.NSeries.CategoryData = "C1:C3";
            
            // Obtener la serie y establecer el efecto 3D
            Series series = chart.NSeries[seriesIndex];
            series.Has3DEffect = true;
            series.Bar3DShapeType = Bar3DShapeType.Cylinder;

            // Guarda el libro de trabajo
            workbook.Save("Series3DEffectDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


