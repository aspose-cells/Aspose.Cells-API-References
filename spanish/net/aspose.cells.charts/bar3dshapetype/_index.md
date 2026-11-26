---
title: "Enum Bar3DShapeType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enum Aspose.Cells.Charts.Bar3DShapeType. Representa la forma utilizada con el gráfico de barras o columnas 3D"
type: docs
url: /es/net/aspose.cells.charts/bar3dshapetype/
---
## Bar3DShapeType enumeration

Representa la forma utilizada con el gráfico de barras o columnas 3D.

```csharp
public enum Bar3DShapeType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Box | `0` | Caja |
| PyramidToPoint | `1` | PyramidToPoint |
| PyramidToMax | `2` | PyramidToMax |
| Cylinder | `3` | Cilindro |
| ConeToPoint | `4` | ConeToPoint |
| ConeToMax | `5` | ConeToMax |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class Bar3DShapeTypeDemo
    {
        public static void Bar3DShapeTypeExample()
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
            worksheet.Cells["A4"].PutValue(200);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);
            worksheet.Cells["B4"].PutValue(40);
            worksheet.Cells["C1"].PutValue("Q1");
            worksheet.Cells["C2"].PutValue("Q2");
            worksheet.Cells["C3"].PutValue("Y1");
            worksheet.Cells["C4"].PutValue("Y2");

            // Agregar un gráfico a la hoja de cálculo
            int chartIndex = worksheet.Charts.Add(ChartType.Column3DClustered, 5, 0, 15, 5);
            // Accediendo a la instancia del gráfico recién agregado
            Chart chart = worksheet.Charts[chartIndex];
            // Agregar NSeries (fuente de datos del gráfico) al gráfico que abarca desde la celda "A1" hasta "B4"
            int seriesIndex = chart.NSeries.Add("A1:B4", true);
            // Estableciendo la fuente de datos para los datos de categoría de NSeries
            chart.NSeries.CategoryData = "C1:C4";
            Series series = chart.NSeries[seriesIndex];
            // Configurando los valores de la serie
            series.Values = "=B1:B4";

            // Configurando el tipo de forma 3D para la serie
            series.Bar3DShapeType = Bar3DShapeType.Cylinder;

            // Guardando el archivo Excel
            workbook.Save("Bar3DShapeTypeExample.xlsx");
            workbook.Save("Bar3DShapeTypeExample.pdf");

            // Configurando el tipo de forma 3D para la serie
            series.Bar3DShapeType = Bar3DShapeType.ConeToMax;

            // Guardando el archivo Excel
            workbook.Save("Bar3DShapeTypeExample2.xlsx");
            workbook.Save("Bar3DShapeTypeExample2.pdf");
            return;
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


