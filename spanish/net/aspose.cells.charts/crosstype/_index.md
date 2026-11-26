---
title: "Enum CrossType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.Charts.CrossType enum. Representa el tipo de cruce del eje"
type: docs
url: /es/net/aspose.cells.charts/crosstype/
---
## CrossType enumeration

Representa el tipo de cruce del eje.

```csharp
public enum CrossType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Automatic | `0` | Microsoft Excel establece el punto de cruce del eje. |
| Maximum | `1` | El eje cruza en el valor máximo. |
| Minimum | `2` | El eje cruza en el valor mínimo. |
| Custom | `3` | El eje cruza en el valor personalizado. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class CrossTypeDemo
    {
        public static void CrossTypeExample()
        {
            // Instanciando un objeto Workbook
            Workbook workbook = new Workbook();
            // Añadiendo una nueva hoja de cálculo al objeto Excel
            int sheetIndex = workbook.Worksheets.Add();
            // Obteniendo la referencia de la hoja de cálculo recién añadida pasando su índice de hoja
            Worksheet worksheet = workbook.Worksheets[sheetIndex];
            // Agregar valores de muestra a celdas
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(4);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(50);

            // Agregar un gráfico a la hoja de cálculo
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 25, 5);
            // Accediendo a la instancia del gráfico recién agregado
            Chart chart = worksheet.Charts[chartIndex];
            // Añadiendo NSeries (fuente de datos del gráfico) al gráfico desde la celda "A1" hasta "B3"
            chart.NSeries.Add("A1:B3", true);

            // Establecer el valor máximo del eje de valores
            chart.ValueAxis.MaxValue = 200;
            // Establecer el valor mínimo del eje de valores
            chart.ValueAxis.MinValue = 0;
            // Establecer la unidad principal
            chart.ValueAxis.MajorUnit = 25;

            // El eje Category(X) cruza en el valor máximo
            chart.ValueAxis.CrossType = CrossType.Maximum;

            // Establecer el número de categorías o series entre las etiquetas de marcas de graduación
            chart.CategoryAxis.TickLabelSpacing = 2;

            // Guardando el archivo Excel
            workbook.Save("CrossTypeExample.xlsx");
            workbook.Save("CrossTypeExample.pdf");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


