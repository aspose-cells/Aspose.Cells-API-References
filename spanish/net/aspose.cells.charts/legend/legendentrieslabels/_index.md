---
title: "Legend.LegendEntriesLabels"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Legend. Obtiene las etiquetas de las entradas de la leyenda después de llamar al método Chart.Calculate"
type: docs
url: /es/net/aspose.cells.charts/legend/legendentrieslabels/
---
## Legend.LegendEntriesLabels property

Obtiene las etiquetas de las entradas de la leyenda después de llamar al método Chart.Calculate().

```csharp
[Obsolete("Use Legend.GetLegendLabels method, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public ArrayList LegendEntriesLabels { get; }
```

### Observaciones

NOTA: Este miembro está ahora obsoleto. En su lugar, por favor use el método Legend.GetLegendLabels. Esta propiedad será eliminada 12 meses después desde noviembre de 2023. Aspose se disculpa por cualquier inconveniente que pueda haber experimentado.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class LegendPropertyLegendEntriesLabelsDemo
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

            // Añade un gráfico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Establecer origen de datos del Chart
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Calcular el gráfico para asegurar que se generen las entradas de la leyenda
            chart.Calculate();

            // Obtener la leyenda
            Legend legend = chart.Legend;

            // Mostrar las etiquetas de las entradas de la leyenda (usando la propiedad)
            Console.WriteLine("Legend Entries Labels:");
            foreach (string label in legend.LegendEntriesLabels)
            {
                Console.WriteLine(label);
            }

            // Guarda el libro de trabajo
            workbook.Save("LegendEntriesLabelsDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Legend](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


