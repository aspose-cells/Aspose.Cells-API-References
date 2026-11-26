---
title: "Axis.AxisLabels"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad del eje. Obtiene las etiquetas del eje después de llamar al método Chart.Calculate"
type: docs
url: /es/net/aspose.cells.charts/axis/axislabels/
---
## Axis.AxisLabels property

Obtiene las etiquetas del eje después de llamar al método Chart.Calculate().

```csharp
[Obsolete("Use Axis.GetAxisTexts method, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public ArrayList AxisLabels { get; }
```

### Observaciones

NOTA: Este miembro está ahora obsoleto. En su lugar, utilice el método Axis.GetAxisTexts. Esta propiedad será eliminada 12 meses después desde noviembre de 2023. Aspose se disculpa por cualquier inconveniente que pueda haber experimentado.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class AxisPropertyAxisLabelsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregue datos de muestra para el gráfico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B4"].PutValue(30);

            try
            {
                // Agregar un gráfico a la hoja de cálculo
                int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
                Chart chart = worksheet.Charts[chartIndex];

                // Establecer rango de datos del gráfico
                chart.NSeries.Add("B2:B4", true);
                chart.NSeries.CategoryData = "A2:A4";

                // Calcular el gráfico para generar etiquetas del eje
                chart.Calculate();

                // Acceder al eje de categorías y obtener las etiquetas del eje
                Axis categoryAxis = chart.CategoryAxis;
                var axisLabels = categoryAxis.AxisLabels;

                // Mostrar las etiquetas del eje
                Console.WriteLine("Axis Labels:");
                if (axisLabels != null)
                {
                    foreach (var label in axisLabels)
                    {
                        Console.WriteLine(label);
                    }
                }
                else
                {
                    Console.WriteLine("No axis labels available.");
                }

                // Guarda el libro de trabajo
                workbook.Save("AxisPropertyAxisLabelsDemo.xlsx");
                Console.WriteLine("AxisLabels demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


