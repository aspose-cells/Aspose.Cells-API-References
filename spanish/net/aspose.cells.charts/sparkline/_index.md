---
title: "Clase Sparkline"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Charts.Sparkline. Un sparkline representa un pequeño gráfico o imagen en una celda de hoja de cálculo que proporciona una representación visual de los datos"
type: docs
url: /es/net/aspose.cells.charts/sparkline/
---
## Sparkline class

Una sparkline representa un pequeño gráfico o imagen en una celda de hoja de cálculo que proporciona una representación visual de los datos.

```csharp
public class Sparkline
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Column](../../aspose.cells.charts/sparkline/column/) { get; } | Obtiene el índice de columna del sparkline. |
| [DataRange](../../aspose.cells.charts/sparkline/datarange/) { get; set; } | Representa el rango de datos del sparkline. |
| [Row](../../aspose.cells.charts/sparkline/row/) { get; } | Obtiene el índice de fila del sparkline. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [ToImage](../../aspose.cells.charts/sparkline/toimage/#toimage)(ImageOrPrintOptions) | Convierte un sparkline a una imagen. |
| [ToImage](../../aspose.cells.charts/sparkline/toimage/#toimage_1)(Stream, ImageOrPrintOptions) | Convierte un sparkline a una imagen. |
| [ToImage](../../aspose.cells.charts/sparkline/toimage/#toimage_2)(string, ImageOrPrintOptions) | Convierte un sparkline a una imagen. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Rendering;
    using System;
    using System.IO;

    public class SparklineDemo
    {
        public static void SparklineExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agregar algunos datos a la hoja de cálculo
            sheet.Cells["A1"].PutValue(5);
            sheet.Cells["B1"].PutValue(2);
            sheet.Cells["C1"].PutValue(1);
            sheet.Cells["D1"].PutValue(3);

            // Define el CellArea para el sparkline
            CellArea ca = new CellArea
            {
                StartColumn = 4,
                EndColumn = 4,
                StartRow = 0,
                EndRow = 0
            };

            // Añade un grupo de sparkline a la hoja de cálculo
            int idx = sheet.SparklineGroups.Add(SparklineType.Line, sheet.Name + "!A1:D1", false, ca);
            SparklineGroup group = sheet.SparklineGroups[idx];

            // Agregar un sparkline al grupo
            idx = group.Sparklines.Add(sheet.Name + "!A1:D1", 0, 5);
            Sparkline line = group.Sparklines[idx];

            // Mostrar detalles del sparkline
            Console.WriteLine("Sparkline data range: " + line.DataRange + ", row: " + line.Row + ", column: " + line.Column);

            // Guardar el sparkline como una imagen
            ImageOrPrintOptions options = new ImageOrPrintOptions
            {
                ImageType = Aspose.Cells.Drawing.ImageType.Png,
                HorizontalResolution = 300,
                VerticalResolution = 300
            };
            line.ToImage("output.png", options);

            // Guarda el libro de trabajo
            workbook.Save("SparklineExample.xlsx");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


