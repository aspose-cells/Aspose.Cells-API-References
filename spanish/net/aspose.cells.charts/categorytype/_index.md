---
title: "Enumeración CategoryType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.Charts.CategoryType enum. Representa el tipo de eje de categorías"
type: docs
url: /es/net/aspose.cells.charts/categorytype/
---
## CategoryType enumeration

Representa el tipo de eje de categoría.

```csharp
public enum CategoryType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| AutomaticScale | `0` | AutomaticScale |
| CategoryScale | `1` | CategoryScale |
| TimeScale | `2` | TimeScale |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class CategoryTypeDemo
    {
        public static void CategoryTypeExample()
        {
            // Instanciando un objeto Workbook
            Workbook workbook = new Workbook();
            // Añadiendo una nueva hoja de cálculo al objeto Excel
            int sheetIndex = workbook.Worksheets.Add();
            // Obteniendo la referencia de la hoja de cálculo recién añadida pasando su índice de hoja
            Worksheet worksheet = workbook.Worksheets[sheetIndex];
            // Agregar valores de muestra a celdas
            worksheet.Cells["A1"].PutValue("Dates");
            worksheet.Cells["A2"].PutValue(new DateOnly(2024, 01, 01));
            worksheet.Cells["A3"].PutValue(new DateOnly(2024, 03, 01));
            worksheet.Cells["A4"].PutValue(new DateOnly(2024, 05, 01));
            worksheet.Cells["B1"].PutValue("Data1");
            worksheet.Cells["B2"].PutValue(4);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(50);
            worksheet.Cells["C1"].PutValue("Data2");
            worksheet.Cells["C2"].PutValue(8);
            worksheet.Cells["C3"].PutValue(15);
            worksheet.Cells["C4"].PutValue(30);

            // Agregar un gráfico a la hoja de cálculo
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 25, 5);
            // Accediendo a la instancia del gráfico recién agregado
            Chart chart = worksheet.Charts[chartIndex];
            // Añadiendo NSeries (fuente de datos del gráfico) al gráfico desde la celda "A1" hasta "B3"
            chart.NSeries.Add("B2:C4", true);

            // Estableciendo los nombres de categoría para el eje X a partir del rango "A2:A5"
            chart.NSeries[0].XValues = "A2:A4";

            // Estableciendo el tipo de eje de categorías a TimeScale
            chart.CategoryAxis.CategoryType = CategoryType.CategoryScale;

            // Estableciendo la escala de unidad mayor para el eje de categorías
            chart.CategoryAxis.MajorUnitScale = TimeUnit.Months;
            chart.CategoryAxis.MajorUnit = 2;

            // Estableciendo la escala de unidad menor para el eje de categorías
            chart.CategoryAxis.MinorUnitScale = TimeUnit.Months;
            chart.CategoryAxis.MinorUnit = 2;

            // Guardando el archivo Excel
            workbook.Save("CategoryTypeExample.xlsx");
            workbook.Save("CategoryTypeExample.pdf");

        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


