---
title: "ChartFrame.AutoScaleFont"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ChartFrame. True si el texto en el objeto cambia el tamaño de fuente cuando el tamaño del objeto cambia. El valor predeterminado es True"
type: docs
url: /es/net/aspose.cells.charts/chartframe/autoscalefont/
---
## ChartFrame.AutoScaleFont property

True si el texto en el objeto cambia el tamaño de fuente cuando cambia el tamaño del objeto. El valor predeterminado es True.

```csharp
public virtual bool AutoScaleFont { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartFramePropertyAutoScaleFontDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregue datos de muestra para el gráfico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Agregar un gráfico a la hoja de cálculo
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Establecer origen de datos del Chart
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Acceder al título del gráfico
            chart.Title.Text = "Sample Chart";
            
            // Demostrar la propiedad AutoScaleFont
            chart.Title.AutoScaleFont = true;
            Console.WriteLine("Chart title AutoScaleFont is set to: " + chart.Title.AutoScaleFont);

            // Guarda el libro de trabajo
            workbook.Save("ChartFrameAutoScaleFontDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


