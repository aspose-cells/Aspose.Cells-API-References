---
title: "Axis.CustUnit"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Axis. Especifica un valor personalizado para la unidad de visualización"
type: docs
url: /es/net/aspose.cells.charts/axis/custunit/
---
## Axis.CustUnit property

Especifica un valor personalizado para la unidad de visualización.

```csharp
[Obsolete("Use Axis.CustomUnit property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int CustUnit { get; set; }
```

### Observaciones

NOTA: Esta propiedad está ahora obsoleta. En su lugar, por favor use la propiedad Axis.CustomUnit. Esta propiedad será eliminada 12 meses después desde enero de 2023. Aspose se disculpa por cualquier inconveniente que pueda haber experimentado.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class AxisPropertyCustUnitDemo
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
            worksheet.Cells["A5"].PutValue("D");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(1000000);
            worksheet.Cells["B3"].PutValue(2000000);
            worksheet.Cells["B4"].PutValue(3000000);
            worksheet.Cells["B5"].PutValue(4000000);

            // Agregar un gráfico y establecer su rango de datos
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B5", true);
            chart.NSeries.CategoryData = "A2:A5";

            // Obtener el eje de valores
            Axis valueAxis = chart.ValueAxis;

            // Mostrar el valor actual de CustUnit (propiedad obsoleta)
            Console.WriteLine("Current CustUnit value: " + valueAxis.CustUnit);

            // Establecer un nuevo valor de unidad personalizada (1,000,000)
            valueAxis.CustUnit = 1000000;
            valueAxis.IsDisplayUnitLabelShown = true;

            // Mostrar el nuevo valor de CustUnit
            Console.WriteLine("New CustUnit value: " + valueAxis.CustUnit);

            // Guardar el resultado
            workbook.Save("AxisPropertyCustUnitDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


