---
title: "Chart.SizeWithWindow"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad del gráfico. Verdadero si Microsoft Excel redimensiona el gráfico para que coincida con el tamaño de la ventana de la hoja del gráfico"
type: docs
url: /es/net/aspose.cells.charts/chart/sizewithwindow/
---
## Chart.SizeWithWindow property

True si Microsoft Excel redimensiona el gráfico para que coincida con el tamaño de la ventana de la hoja del gráfico.

```csharp
public bool SizeWithWindow { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertySizeWithWindowDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo para el gráfico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            
            // Añade un gráfico
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Establecer origen de datos del Chart
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // Demostrar la propiedad SizeWithWindow
            Console.WriteLine("Default SizeWithWindow: " + chart.SizeWithWindow);
            
            // Habilitar SizeWithWindow
            chart.SizeWithWindow = true;
            Console.WriteLine("After setting SizeWithWindow to true: " + chart.SizeWithWindow);
            
            // Guarda el libro de trabajo
            workbook.Save("ChartSizeWithWindowDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


