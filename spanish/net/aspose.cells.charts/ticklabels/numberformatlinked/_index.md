---
title: "TickLabels.NumberFormatLinked"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad TickLabels. True si el formato numérico está vinculado a las celdas de modo que el formato numérico cambie en las etiquetas cuando cambie en las celdas"
type: docs
url: /es/net/aspose.cells.charts/ticklabels/numberformatlinked/
---
## TickLabels.NumberFormatLinked property

True si el formato numérico está vinculado a las celdas (de modo que el formato numérico cambie en las etiquetas cuando cambie en las celdas).

```csharp
public bool NumberFormatLinked { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class TickLabelsPropertyNumberFormatLinkedDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue(100);
            worksheet.Cells["A2"].PutValue(200);
            worksheet.Cells["A3"].PutValue(300);
            worksheet.Cells["A4"].PutValue(400);
            
            // Añade un gráfico
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Establecer origen de datos del Chart
            chart.NSeries.Add("A1:A4", true);
            
            // Acceder a las etiquetas de marcas del eje de valores
            Aspose.Cells.Charts.TickLabels tickLabels = chart.ValueAxis.TickLabels;
            
            // Demostrar la propiedad NumberFormatLinked
            Console.WriteLine("NumberFormatLinked (default): " + tickLabels.NumberFormatLinked);
            
            // Cambiar la propiedad
            tickLabels.NumberFormatLinked = false;
            Console.WriteLine("NumberFormatLinked after change: " + tickLabels.NumberFormatLinked);
            
            // Guarda el libro de trabajo
            workbook.Save("TickLabelsNumberFormatLinkedDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ver también

* class [TickLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


