---
title: "Axis.DisplayUnit"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Axis. Representa la etiqueta de unidad para el eje especificado"
type: docs
url: /es/net/aspose.cells.charts/axis/displayunit/
---
## Axis.DisplayUnit property

Representa la etiqueta de unidad para el eje especificado.

```csharp
public DisplayUnitType DisplayUnit { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyDisplayUnitDemo
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
            worksheet.Cells["B2"].PutValue(10000);
            worksheet.Cells["B3"].PutValue(20000);
            worksheet.Cells["B4"].PutValue(30000);

            // Agregar un gráfico de columnas
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Establecer rango de datos del gráfico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Establecer la unidad de visualización del eje de valores a miles
            chart.ValueAxis.DisplayUnit = DisplayUnitType.Thousands;

            // Guarda el libro de trabajo
            workbook.Save("AxisPropertyDisplayUnitDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ver también

* enum [DisplayUnitType](../../displayunittype/)
* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


