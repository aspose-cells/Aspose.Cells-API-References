---
title: "AxisBins.ResetUnderflow"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método AxisBins. Restablecer el subdesbordamiento"
type: docs
url: /es/net/aspose.cells.charts/axisbins/resetunderflow/
---
## AxisBins.ResetUnderflow method

Restablecer el subdesbordamiento

```csharp
[Obsolete("This is an internal method.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void ResetUnderflow()
```

### Observaciones

NOTA: Este método está ahora obsoleto. Es un método interno que no necesita ser llamado externamente para evitar causar problemas. Esta propiedad será eliminada 12 meses después a partir de julio de 2024. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class AxisBinsMethodResetUnderflowDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
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

            // Crear un gráfico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Obtener el eje de valores
            Axis valueAxis = chart.ValueAxis;
            
            // Crear contenedores de eje
            valueAxis.Bins.IsAutomatic = false;
            valueAxis.Bins.Count = 5;
            valueAxis.Bins.Underflow = 5;
            
            try
            {
                // Llamar al método ResetUnderflow
                valueAxis.Bins.ResetUnderflow();
                
                Console.WriteLine("Underflow value after reset: " + valueAxis.Bins.Underflow);
                
                // Guarda el libro de trabajo
                workbook.Save("AxisBinsMethodResetUnderflowDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ResetUnderflow method: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [AxisBins](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


