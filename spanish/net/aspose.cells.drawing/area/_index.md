---
title: "Clase Area"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Drawing.Area. Encapsula el objeto que representa un formato de área"
type: docs
url: /es/net/aspose.cells.drawing/area/
---
## Area class

Encapsula el objeto que representa un formato de área.

```csharp
public class Area
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [BackgroundColor](../../aspose.cells.drawing/area/backgroundcolor/) { get; set; } | Obtiene o establece el Color de fondo del `Area`. |
| [FillFormat](../../aspose.cells.drawing/area/fillformat/) { get; } | Representa un objeto [`FillFormat`](./fillformat/) que contiene propiedades de formato de relleno para el gráfico o forma especificados. |
| [ForegroundColor](../../aspose.cells.drawing/area/foregroundcolor/) { get; set; } | Obtiene o establece el Color de primer plano. |
| [Formatting](../../aspose.cells.drawing/area/formatting/) { get; set; } | Representa el formato del área. |
| [InvertIfNegative](../../aspose.cells.drawing/area/invertifnegative/) { get; set; } | Si la propiedad es verdadera y el valor del punto del gráfico es un número negativo, el color de primer plano y el color de fondo se intercambiarán. |
| [Transparency](../../aspose.cells.drawing/area/transparency/) { get; set; } | Devuelve o establece el grado de transparencia del área como un valor de 0.0 (opaco) a 1.0 (claro). |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class AreaDemo
    {
        public static void AreaExample()
        {
            // Instanciando un objeto Workbook
            Workbook workbook = new Workbook();
            // Añadiendo una nueva hoja de cálculo al objeto Workbook
            int sheetIndex = workbook.Worksheets.Add();
            // Obteniendo la referencia de la hoja de cálculo recién añadida pasando su índice de hoja
            Worksheet worksheet = workbook.Worksheets[sheetIndex];
            // Agregar valores de muestra a celdas
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(-100);
            worksheet.Cells["A3"].PutValue(150);
            // Agregar un gráfico a la hoja de cálculo
            int chartIndex = worksheet.Charts.Add(ChartType.Area, 5, 0, 15, 5);
            // Accediendo a la instancia del gráfico recién agregado
            Chart chart = worksheet.Charts[chartIndex];
            // Agregando NSeries (fuente de datos del gráfico) al gráfico que abarca desde la celda "A1" hasta "A3"
            chart.NSeries.Add("A1:A3", true);

            // Accediendo al área de la primera NSeries
            Area area = chart.NSeries[0].Area;

            // Estableciendo propiedades
            area.InvertIfNegative = true;
            area.ForegroundColor = Color.Red;
            area.BackgroundColor = Color.Yellow;
            area.Formatting = Aspose.Cells.Charts.FormattingType.Custom;
            area.Transparency = 0.5;

            // Guardando el archivo Excel
            workbook.Save("AreaExample.xlsx");
            workbook.Save("AreaExample.pdf");

        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


