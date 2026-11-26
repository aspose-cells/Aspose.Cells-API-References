---
title: "Enumeración ChartTextDirectionType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.Charts.ChartTextDirectionType enum. Representa el tipo de dirección del texto del gráfico."
type: docs
url: /es/net/aspose.cells.charts/charttextdirectiontype/
---
## ChartTextDirectionType enumeration

Representa el tipo de dirección del texto del gráfico.

```csharp
public enum ChartTextDirectionType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Horizontal | `0` | Tipo de dirección horizontal. |
| Vertical | `1` | Tipo de dirección vertical. |
| Rotate90 | `2` | Rotar un ángulo de noventa grados. |
| Rotate270 | `3` | Rotar un ángulo de 270 grados. |
| Stacked | `4` | Texto apilado. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;
    using System.Drawing;

    public class ChartTextDirectionTypeDemo
    {
        public static void ChartTextDirectionTypeExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Agregar una nueva hoja de cálculo al libro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo a la hoja de cálculo
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
            
            // Agregar series de datos al gráfico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // Establecer el título del gráfico
            chart.Title.Text = "Sample Chart";
            chart.Title.Font.Color = Color.Blue;
            
            // Establecer la dirección del texto del título del gráfico
            chart.Title.DirectionType = ChartTextDirectionType.Rotate90;
            
            // Establecer la dirección del texto del título del eje de categorías
            chart.CategoryAxis.Title.Text = "Categories";
            chart.CategoryAxis.Title.DirectionType = ChartTextDirectionType.Vertical;
            
            // Establecer la dirección del texto del título del eje de valores
            chart.ValueAxis.Title.Text = "Values";
            chart.ValueAxis.Title.DirectionType = ChartTextDirectionType.Horizontal;
            
            // Guarda el libro de trabajo
            workbook.Save("ChartTextDirectionTypeExample.xlsx");
            workbook.Save("ChartTextDirectionTypeExample.pdf");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


