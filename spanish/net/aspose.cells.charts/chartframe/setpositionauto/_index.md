---
title: "ChartFrame.SetPositionAuto"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método ChartFrame. Establecer la posición del marco a automática"
type: docs
url: /es/net/aspose.cells.charts/chartframe/setpositionauto/
---
## ChartFrame.SetPositionAuto method

Establecer la posición del marco a automática

```csharp
public virtual void SetPositionAuto()
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartFrameMethodSetPositionAutoDemo
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
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Establecer origen de datos del Chart
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Obtener el marco del título del gráfico
            ChartFrame title = chart.Title;
            
            // Establecer posición manual primero para demostrar SetPositionAuto
            title.XRatioToChart = 0.2;
            title.YRatioToChart = 0.1;
            title.WidthRatioToChart = 0.6;
            title.HeightRatioToChart = 0.1;

            try
            {
                // Llamar al método SetPositionAuto
                title.SetPositionAuto();
                
                Console.WriteLine("Chart title position set to automatic successfully");
                
                // Mostrar los nuevos valores de posición automática
                Console.WriteLine($"New X position ratio: {title.XRatioToChart}");
                Console.WriteLine($"New Y position ratio: {title.YRatioToChart}");
                Console.WriteLine($"New Width ratio: {title.WidthRatioToChart}");
                Console.WriteLine($"New Height ratio: {title.HeightRatioToChart}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetPositionAuto method: {ex.Message}");
            }
            
            // Guardar el resultado
            workbook.Save("ChartFrameSetPositionAutoDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


