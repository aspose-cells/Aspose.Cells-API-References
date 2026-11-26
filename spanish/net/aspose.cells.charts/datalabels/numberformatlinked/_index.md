---
title: "DataLabels.NumberFormatLinked"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad DataLabels. Verdadero si el formato numérico está vinculado a las celdas de modo que el formato numérico cambie en las etiquetas cuando cambie en las celdas"
type: docs
url: /es/net/aspose.cells.charts/datalabels/numberformatlinked/
---
## DataLabels.NumberFormatLinked property

True si el formato numérico está vinculado a las celdas (de modo que el formato numérico cambie en las etiquetas cuando cambie en las celdas).

```csharp
public bool NumberFormatLinked { get; set; }
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
    public class DataLabelsPropertyNumberFormatLinkedDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["C1"].PutValue("Formatted Value");
            worksheet.Cells["C2"].PutValue("100 units");
            worksheet.Cells["C3"].PutValue("200 units");

            // Crear un gráfico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Agregar serie
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";
            
            // Configurar etiquetas de datos
            var series = chart.NSeries[0];
            series.DataLabels.ShowValue = true;
            series.DataLabels.LinkedSource = "C2:C3";
            series.DataLabels.NumberFormatLinked = true; // Link number format from source cells
            
            // Guarda el libro de trabajo
            workbook.Save("DataLabelsNumberFormatLinkedDemo.xlsx");
        }
    }
}
```

### Ver también

* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


