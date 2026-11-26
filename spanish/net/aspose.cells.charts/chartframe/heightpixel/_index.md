---
title: "ChartFrame.HeightPixel"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ChartFrame. Obtiene o establece la altura del marco en unidades de píxeles"
type: docs
url: /es/net/aspose.cells.charts/chartframe/heightpixel/
---
## ChartFrame.HeightPixel property

Obtiene o establece la altura del marco en unidades de píxeles.

```csharp
public virtual int HeightPixel { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartFramePropertyHeightPixelDemo
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
            
            // Acceder al título del gráfico (que es un ChartFrame)
            ChartFrame chartTitle = chart.Title;
            
            // Mostrar la altura actual en píxeles
            Console.WriteLine("Current title height: " + chartTitle.HeightPixel + " pixels");
            
            // Establecer una nueva altura para el título
            chartTitle.HeightPixel = 40;
            Console.WriteLine("New title height: " + chartTitle.HeightPixel + " pixels");
            
            // Acceder a la leyenda (otro ChartFrame)
            ChartFrame legend = chart.Legend;
            
            // Mostrar y modificar la altura de la leyenda
            Console.WriteLine("Current legend height: " + legend.HeightPixel + " pixels");
            legend.HeightPixel = 60;
            Console.WriteLine("New legend height: " + legend.HeightPixel + " pixels");
            
            // Guarda el libro de trabajo
            workbook.Save("ChartFrameHeightPixelDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


