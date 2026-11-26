---
title: "PlotArea.SetPositionAuto"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método PlotArea. Establecer la posición del área del gráfico a automática"
type: docs
url: /es/net/aspose.cells.charts/plotarea/setpositionauto/
---
## PlotArea.SetPositionAuto method

Establecer la posición del área de trazado a automático

```csharp
public override void SetPositionAuto()
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class PlotAreaMethodSetPositionAutoDemo
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

            try
            {
                // Obtener el área de trazado del gráfico
                PlotArea plotArea = chart.PlotArea;
                
                // Establezca manualmente algunos valores de posición primero para demostrar el efecto
                plotArea.XRatioToChart = 0.1;
                plotArea.YRatioToChart = 0.1;
                plotArea.WidthRatioToChart = 0.8;
                plotArea.HeightRatioToChart = 0.8;
                
                // Llame a SetPositionAuto para restablecer la posición automática
                plotArea.SetPositionAuto();
                
                Console.WriteLine("Plot area position has been set to automatic.");
                
                // Guardar el libro de trabajo para mostrar el efecto
                workbook.Save("PlotAreaSetPositionAutoDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetPositionAuto method: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [PlotArea](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


