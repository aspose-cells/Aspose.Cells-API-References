---
title: "ChartFrame.XPixel"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ChartFrame. Obtiene o establece la coordenada x de la esquina superior izquierda en unidades de píxel"
type: docs
url: /es/net/aspose.cells.charts/chartframe/xpixel/
---
## ChartFrame.XPixel property

Obtiene o establece la coordenada x de la esquina superior izquierda en unidades de píxel.

```csharp
public virtual int XPixel { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartFramePropertyXPixelDemo
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
            
            // Acceder al título del gráfico (que hereda de ChartFrame)
            chart.Title.Text = "Sample Chart";
            
            // Mostrar la posición actual de XPixel del título
            Console.WriteLine("Current Title XPixel position: " + chart.Title.XPixel);
            
            // Mover el título horizontalmente cambiando XPixel
            chart.Title.XPixel = 200;
            
            // Mostrar la nueva posición de XPixel
            Console.WriteLine("New Title XPixel position: " + chart.Title.XPixel);
            
            // Guarda el libro de trabajo
            workbook.Save("ChartFrameXPixelDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


