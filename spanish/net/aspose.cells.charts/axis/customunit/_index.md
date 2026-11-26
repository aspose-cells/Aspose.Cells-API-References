---
title: "Axis.CustomUnit"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Axis. Especifica un valor personalizado para la unidad de visualización"
type: docs
url: /es/net/aspose.cells.charts/axis/customunit/
---
## Axis.CustomUnit property

Especifica un valor personalizado para la unidad de visualización.

```csharp
[Obsolete("Use Axis.CustomDisplayUnit property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int CustomUnit { get; set; }
```

### Observaciones

NOTA: Esta propiedad está ahora obsoleta. En su lugar, utilice la propiedad Axis.CustomDisplayUnit. Esta propiedad será eliminada 12 meses después a partir de febrero de 2025. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class AxisPropertyCustomUnitDemo
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
            worksheet.Cells["B2"].PutValue(1000000);
            worksheet.Cells["B3"].PutValue(2000000);
            worksheet.Cells["B4"].PutValue(3000000);

            // Agregar un gráfico de columnas
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Establecer origen de datos del Chart
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            try
            {
                // Acceder al eje de valores
                Axis valueAxis = chart.ValueAxis;

                // Establecer la unidad de visualización a personalizada
                valueAxis.DisplayUnit = DisplayUnitType.Custom;

                // Establecer el valor de la unidad de visualización personalizada
                valueAxis.CustomDisplayUnit = 1000000;

                // Mostrar el valor de la propiedad CustomUnit (propiedad obsoleta)
                Console.WriteLine("CustomUnit value: " + valueAxis.CustomUnit);

                // Guarda el libro de trabajo
                workbook.Save("AxisPropertyCustomUnitDemo.xlsx");
                Console.WriteLine("CustomUnit has been demonstrated");
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


