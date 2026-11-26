---
title: "Enumeración DataLabelShapeType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enumeración Aspose.Cells.Drawing.DataLabelShapeType. Especifica la geometría de forma predefinida que se debe usar para un gráfico."
type: docs
url: /es/net/aspose.cells.drawing/datalabelshapetype/
---
## DataLabelShapeType enumeration

Especifica la geometría de forma predefinida que se utilizará para un gráfico.

```csharp
public enum DataLabelShapeType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Rect | `0` | Representa la forma rectangular. |
| RoundRect | `1` | Representa la forma de rectángulo redondeado. |
| Ellipse | `2` | Representa la forma de elipse. |
| RightArrowCallout | `3` | Representa la forma de llamada con flecha derecha. |
| DownArrowCallout | `4` | Representa la forma de llamada con flecha hacia abajo. |
| LeftArrowCallout | `5` | Representa la forma de llamada con flecha izquierda. |
| UpArrowCallout | `6` | Representa la forma de llamada con flecha hacia arriba. |
| WedgeRectCallout | `7` | Representa la forma de llamada de cuña rectangular. |
| WedgeRoundRectCallout | `8` | Representa la forma de llamada de cuña con rectángulo redondeado. |
| WedgeEllipseCallout | `9` | Representa la forma de llamada de cuña elíptica. |
| LineCallout | `10` | Representa la forma de llamada de línea. |
| BentLineCallout | `11` | Representa la forma de llamada de línea doblada. |
| LineWithAccentBarCallout | `12` | Representa la forma de llamada de línea con barra de acento. |
| BentLineWithAccentBarCallout | `13` | Representa la forma de llamada de línea doblada con barra de acento. |
| Line | `14` | Este tipo solo se usa para procesamiento de archivos especiales. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;

    public class DataLabelShapeTypeDemo
    {
        public static void DataLabelShapeTypeExample()
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

            // Establecer el rango de datos del gráfico
            chart.SetChartDataRange("A1:B4", true);

            // Acceder a la primera serie del gráfico
            Series series = chart.NSeries[0];

            // Habilitar etiquetas de datos para la serie.
            series.DataLabels.ShowValue = true;
            series.DataLabels.ShapeType = DataLabelShapeType.RoundRect;

            // Guarda el libro de trabajo
            workbook.Save("DataLabelShapeTypeExample.xlsx");
            workbook.Save("DataLabelShapeTypeExample.pdf");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


