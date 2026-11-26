---
title: "LegendEntry.Background"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad LegendEntry. Obtiene y establece el modo de visualización del fondo"
type: docs
url: /es/net/aspose.cells.charts/legendentry/background/
---
## LegendEntry.Background property

Obtiene y establece el modo de visualización del fondo

```csharp
[Obsolete("Use LegendEntry.BackgroundMode property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public BackgroundMode Background { get; set; }
```

### Observaciones

NOTA: Este miembro está ahora obsoleto. En su lugar, utilice la propiedad LegendEntry.BackgroundMode. Esta propiedad será eliminada 12 meses después desde ENERO de 2012. Aspose se disculpa por cualquier inconveniente que pueda haber experimentado.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class LegendEntryPropertyBackgroundDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregue datos de muestra para el gráfico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Q1");
            worksheet.Cells["A3"].PutValue("Q2");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);

            // Agregar un gráfico a la hoja de cálculo
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Establecer origen de datos del Chart
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            try
            {
                // Obtener la primera entrada de leyenda
                LegendEntry legendEntry = chart.Legend.LegendEntries[0];

                // Mostrar el valor actual de la propiedad Background
                Console.WriteLine("Current Background value: " + legendEntry.Background);

                // Establecer un nuevo valor de Background (ya que no es de solo lectura)
                legendEntry.Background = BackgroundMode.Opaque;
                Console.WriteLine("Background after setting to Opaque: " + legendEntry.Background);

                // Establecer otro valor de Background
                legendEntry.Background = BackgroundMode.Transparent;
                Console.WriteLine("Background after setting to Transparent: " + legendEntry.Background);

                // Guarda el libro de trabajo
                workbook.Save("LegendEntryBackgroundDemo.xlsx");
                Console.WriteLine("Background property demonstration completed successfully.");
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

* enum [BackgroundMode](../../backgroundmode/)
* class [LegendEntry](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


