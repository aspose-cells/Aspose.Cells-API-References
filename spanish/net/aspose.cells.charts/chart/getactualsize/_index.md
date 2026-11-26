---
title: "Chart.GetActualSize"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Chart. Obtiene el tamaño real del gráfico en unidades de píxeles"
type: docs
url: /es/net/aspose.cells.charts/chart/getactualsize/
---
## Chart.GetActualSize method

Obtiene el tamaño real del gráfico en unidades de píxeles.

```csharp
public int[] GetActualSize()
```

### Valor de retorno

Tamaño real en una matriz (ancho y alto). [0] es el ancho; [1] es el alto.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartMethodGetActualSizeDemo
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
            
            // Establecer rango de datos del gráfico
            chart.SetChartDataRange("A1:B4", true);
            
            try
            {
                // Llame al método GetActualSize
                int[] actualSize = chart.GetActualSize();
                
                // Mostrar el resultado
                Console.WriteLine($"Actual chart size - Width: {actualSize[0]}px, Height: {actualSize[1]}px");
                
                // Muestre el efecto redimensionando el objeto del gráfico
                chart.ChartObject.Width = actualSize[0];
                chart.ChartObject.Height = actualSize[1];
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetActualSize method: {ex.Message}");
            }
            
            // Guardar el resultado
            workbook.Save("ChartMethodGetActualSizeDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


