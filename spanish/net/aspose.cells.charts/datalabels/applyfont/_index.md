---
title: "DataLabels.ApplyFont"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método DataLabels. Aplicar la fuente de las etiquetas de datos a todos los nodos hijos"
type: docs
url: /es/net/aspose.cells.charts/datalabels/applyfont/
---
## DataLabels.ApplyFont method

Aplica la fuente de las etiquetas de datos a todos los nodos hijos.

```csharp
public void ApplyFont()
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class DataLabelsMethodApplyFontDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo y acceder a la primera hoja de cálculo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo para el gráfico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["A5"].PutValue("D");
            
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            worksheet.Cells["B5"].PutValue(40);

            // Agregar un gráfico a la hoja de cálculo
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Establecer origen de datos del Chart
            chart.NSeries.Add("B2:B5", true);
            chart.NSeries.CategoryData = "A2:A5";
            
            // Mostrar etiquetas de datos
            Series series = chart.NSeries[0];
            series.DataLabels.ShowValue = true;
            
            // Establecer un nuevo color de fuente para las etiquetas de datos
            Color newColor = Color.Green;
            series.DataLabels.Font.Color = newColor;
            
            // Aplicar la configuración de fuente a todas las etiquetas de datos
            series.DataLabels.ApplyFont();
            
            // Guarda el libro de trabajo
            workbook.Save("DataLabelsApplyFontDemo_out.xlsx");
        }
    }
}
```

### Ver también

* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


