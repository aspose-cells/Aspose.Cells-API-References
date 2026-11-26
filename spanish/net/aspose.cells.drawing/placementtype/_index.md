---
title: "Enumeración PlacementType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enumeración Aspose.Cells.Drawing.PlacementType. Representa la forma en que el objeto de dibujo está unido a las celdas debajo de él"
type: docs
url: /es/net/aspose.cells.drawing/placementtype/
---
## PlacementType enumeration

Representa la forma en que el objeto de dibujo está unido a las celdas debajo de él.

```csharp
public enum PlacementType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| FreeFloating | `0` | No mover ni cambiar el tamaño con las celdas. |
| Move | `1` | Mover pero no cambiar el tamaño con las celdas. |
| MoveAndSize | `2` | Mover y cambiar el tamaño con las celdas. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;

    public class PlacementTypeDemo
    {
        public static void PlacementTypeExample()
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

            // Establezca el tipo de ubicación del gráfico
            chart.Placement = PlacementType.MoveAndSize;

            // Salida del tipo de ubicación
            Console.WriteLine("Chart Placement Type: " + chart.Placement);

            // Guarda el libro de trabajo
            workbook.Save("PlacementTypeExample.xlsx");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


