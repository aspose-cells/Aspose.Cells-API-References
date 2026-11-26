---
title: "Enumeración LabelPositionType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.Charts.LabelPositionType enum. Representa el tipo de posición de la etiqueta de datos"
type: docs
url: /es/net/aspose.cells.charts/labelpositiontype/
---
## LabelPositionType enumeration

Representa el tipo de posición de la etiqueta de datos.

```csharp
public enum LabelPositionType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Center | `0` | Se aplica solo a gráficos de barras, de pastel 2D/3D |
| InsideBase | `1` | Se aplica solo a gráficos de barras, de pastel 2D/3D |
| InsideEnd | `2` | Se aplica solo a gráficos de barras |
| OutsideEnd | `3` | Se aplica solo a gráficos de barras, de pastel 2d/3d |
| Above | `4` | Se aplica solo a gráficos de líneas |
| Below | `5` | Se aplica solo a gráficos de líneas |
| Left | `6` | Se aplica solo a gráficos de líneas |
| Right | `7` | Se aplica solo a gráficos de líneas |
| BestFit | `8` | Se aplica solo a gráficos de pastel 2D/3D |
| Moved | `9` | El usuario movió las etiquetas de datos. Esto es solo para leer el gráfico del archivo de plantilla. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class LabelPositionTypeDemo
    {
        public static void LabelPositionTypeExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agrega algunos datos de muestra para el gráfico
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

            // Agregar la serie de datos al gráfico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Acceder a las DataLabels de la primera serie
            DataLabels dataLabels = chart.NSeries[0].DataLabels;

            // Establecer la posición de las etiquetas de datos
            dataLabels.Position = LabelPositionType.InsideBase;

            // Mostrar el nombre de la categoría en las etiquetas de datos
            dataLabels.ShowCategoryName = true;

            // Mostrar el valor en las etiquetas de datos
            dataLabels.ShowValue = true;

            // Guarda el libro de trabajo
            workbook.Save("LabelPositionTypeExample.xlsx");
            workbook.Save("LabelPositionTypeExample.pdf");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


