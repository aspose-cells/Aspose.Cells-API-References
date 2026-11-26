---
title: "TickLabels.Font"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad TickLabels. Devuelve un objeto Font que representa la fuente del objeto TickLabels especificado"
type: docs
url: /es/net/aspose.cells.charts/ticklabels/font/
---
## TickLabels.Font property

Devuelve un objeto `Font` que representa la fuente del objeto TickLabels especificado.

```csharp
public Font Font { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class TickLabelsPropertyFontDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Category 1");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(20);
            worksheet.Cells["A4"].PutValue(30);
            
            // Añade un gráfico
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Establecer origen de datos del Chart
            chart.NSeries.Add("A2:A4", true);
            chart.NSeries.CategoryData = "A1:A1";
            
            // Acceder a la fuente de las etiquetas de tick
            Aspose.Cells.Charts.TickLabels tickLabels = chart.CategoryAxis.TickLabels;
            Font font = tickLabels.Font;
            
            // Establecer propiedades de fuente
            font.Name = "Arial";
            font.Size = 12;
            font.IsBold = true;
            
            // Guarda el libro de trabajo
            workbook.Save("TickLabelsFontDemo.xlsx");
            
            Console.WriteLine("TickLabels font properties set successfully.");
        }
    }
}
```

### Ver también

* class [Font](../../../aspose.cells/font/)
* class [TickLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


