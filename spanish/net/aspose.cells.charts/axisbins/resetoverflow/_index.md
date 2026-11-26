---
title: "AxisBins.ResetOverflow"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método AxisBins. Restablecer el desbordamiento"
type: docs
url: /es/net/aspose.cells.charts/axisbins/resetoverflow/
---
## AxisBins.ResetOverflow method

Restablecer el desbordamiento

```csharp
[Obsolete("This is an internal method.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void ResetOverflow()
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

    public class AxisBinsMethodResetOverflowDemo
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
            AxisBins bins = valueAxis.Bins;

            // Establecer valor de desbordamiento
            bins.Overflow = 25;
            Console.WriteLine($"Overflow before reset: {bins.Overflow}");

            try
            {
                // Llamar al método ResetOverflow
                bins.ResetOverflow();
                Console.WriteLine($"Overflow after reset: {bins.Overflow}");
                Console.WriteLine("ResetOverflow method executed successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ResetOverflow method: {ex.Message}");
            }

            // Guardar el resultado
            workbook.Save("AxisBinsMethodResetOverflowDemo.xlsx");
        }
    }
}
```

### Ver también

* class [AxisBins](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


