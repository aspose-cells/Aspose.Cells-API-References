---
title: "TickLabels.AutoScaleFont"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad TickLabels. Verdadero si el texto en el objeto cambia el tamaño de fuente cuando cambia el tamaño del objeto. El valor predeterminado es Verdadero"
type: docs
url: /es/net/aspose.cells.charts/ticklabels/autoscalefont/
---
## TickLabels.AutoScaleFont property

True si el texto en el objeto cambia el tamaño de fuente cuando cambia el tamaño del objeto. El valor predeterminado es True.

```csharp
public bool AutoScaleFont { get; set; }
```

### Ejemplos

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class TickLabelsPropertyAutoScaleFontDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            Cells cells = sheet.Cells;

            // Datos de ejemplo
            cells["A1"].PutValue("Region");
            cells["A2"].PutValue("France");
            cells["A3"].PutValue("Germany");
            cells["A4"].PutValue("England");
            cells["B1"].PutValue("Sales");
            cells["B2"].PutValue(100000);
            cells["B3"].PutValue(150000);
            cells["B4"].PutValue(90000);

            // Crear gráfico
            int chartIndex = sheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 1, 20, 10);
            Aspose.Cells.Charts.Chart chart = sheet.Charts[chartIndex];
            
            // Configurar datos del gráfico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // Configurar etiquetas de eje con AutoScaleFont
            chart.CategoryAxis.TickLabels.AutoScaleFont = true;
            chart.CategoryAxis.TickLabels.Font.Size = 12; // Initial size
            
            // Guarda el libro de trabajo
            workbook.Save("TickLabelsAutoScaleFontDemo.xlsx");
        }
    }
}
```

### Ver también

* class [TickLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


